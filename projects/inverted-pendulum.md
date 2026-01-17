---
layout: default
title: 2-Wheel Inverted Pendulum
---

<section class="section-card">
  <h2>2-Wheel Inverted Pendulum</h2>
  <p class="tagline">Self-balancing platform with state-space control and iterative tuning.</p>
  <img src="{{ '/assets/projects/inverted-pendulum.svg' | relative_url }}" alt="Inverted pendulum project placeholder">
</section>

<section class="section-card">
  <h2>Overview</h2>
  <p>I modeled the nonlinear dynamics, linearized the system around the upright equilibrium, and implemented LQR and PID controllers on embedded hardware.</p>
</section>

<section class="section-card">
  <h2>Highlights</h2>
  <ul>
    <li>Derived equations of motion and built a MATLAB/Simulink model.</li>
    <li>Designed a control stack with IMU fusion and motor control.</li>
    <li>Validated stability with step-response testing and disturbance rejection.</li>
  </ul>
</section>
