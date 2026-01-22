---
layout: default
title: Home
---

<section class="hero">
  <div>
    <h2>I believe that when you have a good idea, you are obligated to humanity to bring it to life. That belief is what pushed me toward engineering and keeps me excited about turning concepts into hardware you can touch, test, and improve.
  </h2>
    <p>I am eager to contribute to a team of curious, driven people who care about building valuable, high-quality innovations and are willing to iterate until the details are right.</p>
    <div class="hero-actions">
      <a class="button" href="{{ '/projects.html' | relative_url }}">View Projects</a>
      <a class="button secondary" href="{{ '/resume.html' | relative_url }}">Download Resume</a>
    </div>
  </div>
  <div class="hero-side">
    <img class="profile-photo" src="{{ '/IMG_0819.jpeg' | relative_url }}" alt="Portrait of Adam Vaughan">
    <div class="stats">
      <div class="stat-card">
        <strong>3+</strong>
        <span>Prototype systems built</span>
      </div>
      <div class="stat-card">
        <strong>4</strong>
        <span>Core focus areas: robotics, controls, design, testing</span>
      </div>
      <div class="stat-card">
        <strong>2</strong>
        <span>Research + industry collaborations</span>
      </div>
      <div class="stat-card">
        <strong>100%</strong>
        <span>Hands-on: CAD, fabrication, validation</span>
      </div>
    </div>
  </div>
</section>

<section class="section-card">
  <h2>Featured Work</h2>
  <p class="tagline">A glimpse of projects that combine modeling, control, and mechanical design. Click a title for the full case study.</p>
  <div class="projects-grid">
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/c-clamp.html' | relative_url }}">
        <img src="{{ '/assets/projects/robotic-arm.svg' | relative_url }}" alt="C-clamp project placeholder">
        <h3>C-Clamp</h3>
        <div class="project-meta">Mechanical Design</div>
        <p class="tagline">Design for strength, manufacturability, and reliable clamping performance.</p>
      </a>
    </article>
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/phone-gimbal.html' | relative_url }}">
        <img src="{{ '/assets/projects/active-noise.svg' | relative_url }}" alt="Phone gimbal project placeholder">
        <h3>Phone Gimbal</h3>
        <div class="project-meta">Mechatronics</div>
        <p class="tagline">Compact stabilization with smooth motion control and balanced mechanical layout.</p>
      </a>
    </article>
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/turret-guided-laser-pointer.html' | relative_url }}">
        <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Turret-guided laser pointer project placeholder">
        <h3>Turret-Guided Laser Pointer</h3>
        <div class="project-meta">Controls + Tracking</div>
        <p class="tagline">Target tracking with a pan-tilt turret and precision alignment logic.</p>
      </a>
    </article>
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/self-balancing-robot.html' | relative_url }}">
        <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Self-balancing robot project placeholder">
        <h3>Self-Balancing Robot</h3>
        <div class="project-meta">Controls + Dynamics</div>
        <p class="tagline">Sensing, estimation, and balance control on a two-wheel platform.</p>
      </a>
    </article>
  </div>
</section>

<section class="section-card">
  <h2>Why I build</h2>
  <p class="tagline">I love projects where mechanical intuition meets data. Whether it is balancing a platform or tuning a noisy system, I document my process and keep design decisions transparent.</p>
  <p class="tagline">I believe that when you have a good idea, you have a responsibility to bring it into the real world, and I am eager to collaborate with people who share that drive to build high-quality, meaningful innovations.</p>
  <a class="button secondary" href="{{ '/about.html' | relative_url }}">Read My Story</a>
</section>
