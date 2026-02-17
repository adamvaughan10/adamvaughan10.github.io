---
layout: default
title: Image Viewer
---

<section class="section-card viewer-header">
  <h2 class="viewer-title">Image Preview</h2>
  <p class="tagline viewer-meta">Loading image…</p>
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
    const isPng = (value) => value && value.toLowerCase().includes('.png');

    if (!src || !isPng(src)) {
      title.textContent = 'Image not found';
      meta.textContent = 'No PNG image was provided.';
      image.remove();
      return;
    }

    image.src = src;
    image.alt = caption || 'Image preview';
    title.textContent = caption || 'Image Preview';
    meta.textContent = caption || src.split('/').pop();
  })();
</script>
