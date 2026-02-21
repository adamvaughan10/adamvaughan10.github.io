---
layout: default
title: Home
---

<section class="hero">
  <div>
  <h2>Mechanical Engineering student ready to build</h2>
  <p>I believe that when you have a good idea, you are obligated to humanity to bring it to life. That belief is what pushed me toward engineering and keeps me excited about turning concepts into hardware you can touch, test, and improve.
  </p>
    <p>I am eager to contribute to a team of curious, driven people who care about building valuable, high-quality innovations and are willing to iterate until the details are right.</p>
    <div class="hero-actions">
      <a class="button" href="{{ '/projects.html' | relative_url }}">View Projects</a>
      <a class="button secondary" href="{{ '/resume.html' | relative_url }}">View Resume</a>
    </div>
  </div>
  <div class="hero-side">
    <img class="profile-photo" src="{{ '/profile.jpeg' | relative_url }}" alt="Portrait of Adam Vaughan">
    
  </div>
</section>

<section class="section-card">
  <h2>Featured Work</h2>
  <p class="tagline">A glimpse of projects that combine modeling, control, and mechanical design. Click a title for the full case study.</p>
  <div class="projects-grid">
    <!--
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/meshiq-mcp-chatbot.html' | relative_url }}">
        <img src="{{ '/assets/projects/meshIQ/cover.png' | relative_url }}" alt="meshIQ MCP chatbot project tile image">
        <h3>AI Chatbot with MCP Integration</h3>
        <div class="project-meta">LLM Systems</div>
        <p class="tagline">Slack-based MCP chatbot for natural-language access to meshIQ data.</p>
      </a>
    </article>
    -->
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/c-clamp.html' | relative_url }}">
        <img src="{{ '/assets/projects/c-clamp/clamp_cover.png' | relative_url }}" alt="C-clamp cover photo">
        <h3>C-Clamp</h3>
        <div class="project-meta">Mechanical Design</div>
        <p class="tagline">Design for strength, manufacturability, and reliable clamping performance.</p>
      </a>
    </article>
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/phone-gimbal.html' | relative_url }}">
        <img src="{{ '/assets/projects/gimbal/title_gimbal.png' | relative_url }}" alt="Phone gimbal project tile image">
        <h3>Phone Gimbal</h3>
        <div class="project-meta">Mechanical Design</div>
        <p class="tagline">Compact stabilization with smooth motion control and balanced mechanical layout.</p>
      </a>
    </article>
    <article class="project-card">
      <a class="project-card-link" href="{{ '/projects/turret-guided-laser-pointer.html' | relative_url }}">
        <img src="{{ '/assets/projects/laser pointer/laserPointerCover.png' | relative_url }}" alt="Turret-guided laser pointer cover image">
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
