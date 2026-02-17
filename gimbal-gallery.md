---
layout: default
title: Phone Gimbal Gallery
---

<section class="section-card">
  <h2>Phone Gimbal Gallery</h2>
  <p><a href="{{ '/projects/phone-gimbal.html' | relative_url }}">&larr; Back to Project</a></p>
</section>

<section class="section-card gallery-container">
  <div class="gallery-grid">
    <figure class="gallery-item">
      <button class="gallery-trigger" data-full="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143701_Notein.jpg' | relative_url }}" data-caption="Design Overview" aria-label="Open Design Overview preview">
        <img src="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143701_Notein.jpg' | relative_url }}" alt="Phone Gimbal - Design Overview" class="gallery-image">
      </button>
      <figcaption>Design Overview</figcaption>
    </figure>
    <figure class="gallery-item">
      <button class="gallery-trigger" data-full="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143720_Notein.jpg' | relative_url }}" data-caption="Handle Assembly" aria-label="Open Handle Assembly preview">
        <img src="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143720_Notein.jpg' | relative_url }}" alt="Phone Gimbal - Handle Assembly" class="gallery-image">
      </button>
      <figcaption>Handle Assembly</figcaption>
    </figure>
    <figure class="gallery-item">
      <button class="gallery-trigger" data-full="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143736_Notein.jpg' | relative_url }}" data-caption="Gimbal Mechanism" aria-label="Open Gimbal Mechanism preview">
        <img src="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143736_Notein.jpg' | relative_url }}" alt="Phone Gimbal - Gimbal Mechanism" class="gallery-image">
      </button>
      <figcaption>Gimbal Mechanism</figcaption>
    </figure>
    <figure class="gallery-item">
      <button class="gallery-trigger" data-full="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143801_Notein.jpg' | relative_url }}" data-caption="Phone Mount Assembly" aria-label="Open Phone Mount Assembly preview">
        <img src="{{ '/assets/projects/gimbal/gallery/Screenshot_20260201_143801_Notein.jpg' | relative_url }}" alt="Phone Gimbal - Phone Mount" class="gallery-image">
      </button>
      <figcaption>Phone Mount Assembly</figcaption>
    </figure>
  </div>
</section>

<div class="lightbox" id="lightbox" aria-hidden="true">
  <div class="lightbox-content" role="dialog" aria-modal="true" aria-label="Image preview">
    <button class="lightbox-close" type="button">Close</button>
    <img class="lightbox-image" src="" alt="">
    <p class="lightbox-caption"></p>
  </div>
</div>

<script>
  const lightbox = document.getElementById('lightbox');
  const lightboxImage = lightbox.querySelector('.lightbox-image');
  const lightboxCaption = lightbox.querySelector('.lightbox-caption');
  const lightboxClose = lightbox.querySelector('.lightbox-close');
  const triggers = document.querySelectorAll('.gallery-trigger');

  const openLightbox = (trigger) => {
    const img = trigger.querySelector('img');
    lightboxImage.src = trigger.dataset.full || img.src;
    lightboxImage.alt = img.alt || '';
    lightboxCaption.textContent = trigger.dataset.caption || '';
    lightbox.classList.add('is-open');
    lightbox.setAttribute('aria-hidden', 'false');
    document.body.style.overflow = 'hidden';
  };

  const closeLightbox = () => {
    lightbox.classList.remove('is-open');
    lightbox.setAttribute('aria-hidden', 'true');
    lightboxImage.src = '';
    document.body.style.overflow = '';
  };

  triggers.forEach((trigger) => {
    trigger.addEventListener('click', () => openLightbox(trigger));
  });

  lightboxClose.addEventListener('click', closeLightbox);
  lightbox.addEventListener('click', (event) => {
    if (event.target === lightbox) {
      closeLightbox();
    }
  });

  document.addEventListener('keydown', (event) => {
    if (event.key === 'Escape' && lightbox.classList.contains('is-open')) {
      closeLightbox();
    }
  });
</script>
