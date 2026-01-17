---
layout: default
title: Projects
---

<section class="section-card">
  <h2>Projects</h2>
  <p class="tagline">Each project includes a short summary, a photo, and a full write-up with modeling, design, and results.</p>
</section>

<section class="section-card">
  <div class="projects-grid">
    <article class="project-card">
      <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Inverted pendulum project placeholder">
      <div class="project-meta">Controls + Dynamics</div>
      <h3><a href="{{ '/projects/inverted-pendulum.html' | relative_url }}">2-Wheel Inverted Pendulum</a></h3>
      <p class="tagline">Linearized dynamics, state-space modeling, and LQR/PID control on a self-balancing platform.</p>
    </article>
    <article class="project-card">
      <img src="{{ '/assets/projects/robotic-arm.svg' | relative_url }}" alt="Robotic arm project placeholder">
      <div class="project-meta">Kinematics + CAD</div>
      <h3><a href="{{ '/projects/robotic-arm.html' | relative_url }}">Robotic Arm Kinematics</a></h3>
      <p class="tagline">DH parameter modeling, inverse kinematics, and MATLAB validation for a 4-DOF arm.</p>
    </article>
    <article class="project-card">
      <img src="{{ '/assets/projects/active-noise.svg' | relative_url }}" alt="Active noise cancellation project placeholder">
      <div class="project-meta">Signal Processing</div>
      <h3><a href="{{ '/projects/active-noise.html' | relative_url }}">Active Noise Cancellation</a></h3>
      <p class="tagline">Real-time signal processing with embedded deployment and experimental verification.</p>
    </article>
  </div>
</section>
