---
layout: default
title: Phone Gimbal
---

<section class="section-card">
  <h2>Phone Stabilizing Gimbal</h2>
  <p class="tagline">Completed Design for Manufacturing (DFM).</p>
</section>

<section class="section-card">
  <h3>Project Snapshot</h3>
  <ul>
    <li><strong>Project:</strong> Phone Stabilizing Gimbal</li>
    <li><strong>Role:</strong> Mechanical Design Engineer (team of two)</li>
    <li><strong>Tools:</strong> SolidWorks</li>
    <li><strong>Status:</strong> Completed design, manufacturing-ready</li>
    <li><strong>Focus:</strong> Mechanical design and DFM (electronics and software considered, not designed)</li>
  </ul>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/gimbal/drawings/MAIN_FINAL.png' | relative_url }}" alt="Phone gimbal main assembly drawing">
    <figcaption class="tagline">Main assembly drawing.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Engineering Considerations</h3>
  <p>The design started with a clear performance target: cinematic stabilization for phones, not just casual handheld smoothing. That meant prioritizing full 3-axis freedom, fast response, and a mass range that would cover today’s heaviest phones while leaving headroom for accessories.</p>
  <ul>
    <li><strong>Stability + control:</strong> Two-handed operation for steadier shots and room for controls, without exceeding a comfortable overall weight.</li>
    <li><strong>Motion envelope:</strong> Motor placement and arm geometry sized to preserve yaw, roll, and pitch travel without self-collision.</li>
    <li><strong>Durability:</strong> Environmental sealing and drop resilience informed material choice, wall thicknesses, and fastener strategy.</li>
    <li><strong>User setup:</strong> A quick-lock clamp sized for a wide phone range, plus clearance for lens rigs.</li>
    <li><strong>Power strategy:</strong> Battery placement and routing planned for long runtime and serviceability without compromising balance.</li>
  </ul>
  <p>Electronics and software were treated as system-level constraints, not fully developed subsystems.</p>
  <p>To view the full spec sheet that we laid out at the beginning of the design process, click on the <a href="{{ '/projects/gimbal-spec-sheet.html' | relative_url }}">link</a>.</p>
</section>

<section class="section-card">
  <h3>Design Approach</h3>
  <ul>
    <li><strong>Requirements first:</strong> Used the spec sheet to set the motion envelope, payload target, and environmental goals before sketching form factors.</li>
    <li><strong>Architecture lock-in:</strong> Committed early to a two-handed frame to stabilize longer shots and give room for a larger power system.</li>
    <li><strong>Mechanism layout:</strong> Sequenced the gimbal axes to preserve full rotation while keeping the phone’s center of mass close to the axis stack.</li>
    <li><strong>Manufacturing intent:</strong> Chose 6061 aluminum for stiffness-to-weight, then shaped parts around standard machining processes.</li>
    <li><strong>Usability details:</strong> Quick-lock phone mounting, grip sizing, and internal routing were refined alongside the CAD assemblies.</li>
  </ul>
  <p><a href="{{ '/gimbal-gallery.html' | relative_url }}">View Gallery →</a></p>
</section>

<section class="section-card">
  <h3>Mechanical Design &amp; CAD</h3>
  <ul>
    <li><strong>Handle assembly:</strong> Ergonomics, rigidity, and internal routing.</li>
    <li><strong>Gimbal assembly:</strong> Isolates and supports phone mount.</li>
    <li><strong>Phone mount assembly:</strong> Most complex component; accommodates a range of phone sizes.</li>
  </ul>
  <p>A full parametric CAD model was developed in SolidWorks with attention to assembly interfaces and manufacturability.</p>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/gimbal/cross_section.png' | relative_url }}" alt="Cross-section of the phone mount showing internal geometry">
    <figcaption class="tagline">Cross-section of the phone mount showing internal geometry and constraints.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Manufacturing &amp; Drawings</h3>
  <ul>
    <li>Manufacturing considerations integrated throughout the design process.</li>
    <li>Detailed engineering drawings created for all machined components.</li>
    <li>GD&amp;T applied to control critical fits, alignment, and functional interfaces.</li>
    <li>Part geometry compatible with standard machining processes.</li>
  </ul>
  <p>Final deliverables support direct handoff to manufacturing.</p>
  <p><a href="{{ '/gimbal-drawings-gallery.html' | relative_url }}">View Drawings Gallery →</a></p>
  <p><a href="{{ '/projects/gimbal-assembly-guide.html' | relative_url }}">View Assembly Guide →</a></p>
</section>

<section class="section-card">
  <h3>Outcome</h3>
  <ul>
    <li>Completed, manufacturing-ready mechanical design.</li>
    <li>Demonstrated concept-to-finalized design execution.</li>
    <li>Documented architectural tradeoffs and DFM decisions.</li>
    <li>Produced professional CAD assemblies and technical drawings.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Key Skills Demonstrated</h3>
  <ul>
    <li>Mechanical design and product development</li>
    <li>Design for Manufacturing (DFM)</li>
    <li>SolidWorks (part modeling, assemblies, drawings)</li>
    <li>GD&amp;T application</li>
    <li>Engineering tradeoff analysis and iteration</li>
  </ul>
</section>
