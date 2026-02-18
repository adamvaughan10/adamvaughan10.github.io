---
layout: default
title: Turret-Guided Laser Pointer
---

<section class="section-card">
  <h2>Turret-Guided Laser Pointer</h2>
  <p class="tagline">A computer-controlled laser pointer exploring pan-tilt actuation, vision feedback, and precision alignment.</p>
</section>

<section class="section-card">
  <h3>Project Snapshot</h3>
  <ul>
    <li><strong>Goal:</strong> Build a laser pointer controllable from a computer, where a user clicks on a camera feed and the laser moves to that location.</li>
    <li><strong>Role:</strong> Solo project (mechanical design, electronics integration, and control logic).</li>
    <li><strong>Tools:</strong> SolidWorks, FDM 3D printing, Raspberry Pi, hobby servos.</li>
    <li><strong>Status:</strong> Functional pan-tilt turret; full closed-loop targeting not achieved.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Design Goals</h3>
  <ul>
    <li><strong>Mechanical:</strong> Design a compact pan-tilt mount using parts on hand (servos + laser pointer).</li>
    <li><strong>Systems:</strong> Learn Raspberry Pi integration, basic electronics, and camera-driven control logic.</li>
    <li><strong>Fabrication:</strong> Use 3D printing to build, iterate, and validate tolerances.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Mechanical Design &amp; 3D Printing</h3>
  <ul>
    <li><strong>CAD:</strong> Designed a full turret assembly in SolidWorks sized around the existing servo motors and laser pointer.</li>
    <li><strong>Fit validation:</strong> Printed test parts to check tolerances, especially the laser pointer holder.</li>
    <li><strong>Tolerance tuning:</strong> Adjusted servo mounting hole sizes to account for 3D printer accuracy.</li>
    <li><strong>Laser mount:</strong> Used a set-screw design; the front set screw also actuated the laser switch.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Electronics &amp; System Setup</h3>
  <ul>
    <li><strong>Controller:</strong> Raspberry Pi as the main control computer.</li>
    <li><strong>Actuation:</strong> Two hobby servos for pan and tilt.</li>
    <li><strong>Power:</strong> External power supply dedicated to the servos.</li>
    <li><strong>Vision:</strong> Logitech camera for live video input.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Control Approach</h3>
  <ul>
    <li><strong>Input:</strong> Intended to map user clicks on the camera feed to target angles.</li>
    <li><strong>Open-loop success:</strong> Achieved turret-like movements and manual positioning.</li>
    <li><strong>Closed-loop attempt:</strong> Tried to detect the laser position and drive to the selected location.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Testing &amp; Issues</h3>
  <ul>
    <li><strong>Geometry limitation:</strong> The camera was too close to the target screen, so click spacing mapped to very small servo movements.</li>
    <li><strong>Power limitation:</strong> The laser was not strong enough to support a larger standoff distance.</li>
    <li><strong>Servo resolution:</strong> Low-resolution hobby servos produced non-repeatable motion with several degrees of variance.</li>
    <li><strong>Result:</strong> Repeatability errors caused large discrepancies in closed-loop targeting.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Outcomes</h3>
  <ul>
    <li>Built a working pan-tilt turret and validated 3D printed fitment.</li>
    <li>Integrated Raspberry Pi control, camera input, and external power for servos.</li>
    <li>Identified the key constraints limiting accurate click-to-point behavior.</li>
  </ul>
</section>

<section class="section-card">
  <h3>What I Learned</h3>
  <ul>
    <li><strong>3D printing:</strong> Real-world tolerance tuning is critical for servo fits and sliding interfaces.</li>
    <li><strong>Systems thinking:</strong> Geometry, optics, and actuator resolution all bound closed-loop performance.</li>
    <li><strong>Electronics:</strong> Separate power domains and proper wiring are essential for reliable servo control.</li>
  </ul>
</section>

<section class="section-card">
  <h3>What I Would Improve Next</h3>
  <ul>
    <li>Use higher-resolution digital servos for repeatable positioning.</li>
    <li>Increase laser brightness to allow a longer standoff distance.</li>
    <li>Add a more accurate calibration routine for pixel-to-angle mapping.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Skills Highlight</h3>
  <ul>
    <li>Mechanical design (SolidWorks)</li>
    <li>FDM 3D printing and tolerance iteration</li>
    <li>Raspberry Pi integration</li>
    <li>Electronics wiring and power planning</li>
    <li>Control system prototyping</li>
  </ul>
</section>
