---
layout: default
title: Home
---

<section class="hero">
  <div>
    <h2>Mechanical engineering student designing machines that feel alive.</h2>
    <p>I focus on robotics, dynamic systems, and control—building prototypes that move with intention and documenting the engineering behind them.</p>
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
      <img src="{{ '/assets/projects/robotic-arm.svg' | relative_url }}" alt="C-clamp project placeholder">
      <div class="project-meta">Mechanical Design</div>
      <h3><a href="{{ '/projects/c-clamp.html' | relative_url }}">C-Clamp</a></h3>
      <p class="tagline">Design for strength, manufacturability, and reliable clamping performance.</p>
    </article>
    <article class="project-card">
      <img src="{{ '/assets/projects/active-noise.svg' | relative_url }}" alt="Phone gimbal project placeholder">
      <div class="project-meta">Mechatronics</div>
      <h3><a href="{{ '/projects/phone-gimbal.html' | relative_url }}">Phone Gimbal</a></h3>
      <p class="tagline">Compact stabilization with smooth motion control and balanced mechanical layout.</p>
    </article>
    <article class="project-card">
      <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Turret-guided laser pointer project placeholder">
      <div class="project-meta">Controls + Tracking</div>
      <h3><a href="{{ '/projects/turret-guided-laser-pointer.html' | relative_url }}">Turret-Guided Laser Pointer</a></h3>
      <p class="tagline">Target tracking with a pan-tilt turret and precision alignment logic.</p>
    </article>
    <article class="project-card">
      <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Self-balancing robot project placeholder">
      <div class="project-meta">Controls + Dynamics</div>
      <h3><a href="{{ '/projects/self-balancing-robot.html' | relative_url }}">Self-Balancing Robot</a></h3>
      <p class="tagline">Sensing, estimation, and balance control on a two-wheel platform.</p>
    </article>
  </div>
</section>

<section class="section-card">
  <h2>Why I build</h2>
  <p class="tagline">I love projects where mechanical intuition meets data. Whether it is balancing a platform or tuning a noisy system, I document my process and keep design decisions transparent.</p>
  <a class="button secondary" href="{{ '/about.html' | relative_url }}">Read My Story</a>
</section>
