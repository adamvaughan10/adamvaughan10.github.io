---
layout: default
title: Image Viewer
---

<section class="section-card viewer-header">
  <h2 class="viewer-title">Image Preview</h2>
  <p class="tagline viewer-meta">Loading image…</p>
  <a class="button secondary viewer-back" href="{{ '/' | relative_url }}">Back to Previous Page</a>
</section>

<section class="section-card viewer-card">
  <div class="viewer-frame">
    <img class="viewer-image" src="" alt="">
  </div>
</section>

<script>
  (() => {
    const params = new URLSearchParams(window.location.search);
    const src = params.get('src');
    const caption = params.get('caption');
    const image = document.querySelector('.viewer-image');
    const title = document.querySelector('.viewer-title');
    const meta = document.querySelector('.viewer-meta');
    const isImage = (value) => {
      if (!value) {
        return false;
      }
      try {
        const path = new URL(value, window.location.origin).pathname.toLowerCase();
        return path.endsWith('.png') || path.endsWith('.jpg') || path.endsWith('.jpeg') || path.endsWith('.webp');
      } catch {
        return false;
      }
    };
    const backLink = document.querySelector('.viewer-back');
    if (document.referrer) {
      try {
        const referrerUrl = new URL(document.referrer);
        if (referrerUrl.origin === window.location.origin) {
          backLink.href = referrerUrl.pathname + referrerUrl.search + referrerUrl.hash;
        }
      } catch {
        // Keep default back link if referrer is invalid.
      }
    }

    if (!src || !isImage(src)) {
      title.textContent = 'Image not found';
      meta.textContent = 'No image was provided.';
      image.remove();
      return;
    }

    image.src = src;
    image.alt = caption || 'Image preview';
    title.textContent = caption || 'Image Preview';
    meta.textContent = caption || src.split('/').pop();
  })();
</script>
