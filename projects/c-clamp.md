---
layout: default
title: C-Clamp
---

<section class="section-card">
  <h2>C-Clamp Manufacturing Project</h2>
  <h3>Project Snapshot</h3>
  <div class="media-block media-left">
    <figure class="media-figure media-figure-small media-figure-rotate-left">
      <img src="{{ '/assets/projects/c-clamp/full.png' | relative_url }}" alt="Full C-clamp assembly">
      <figcaption class="tagline">Full assembly of the C-clamp after fabrication and testing.</figcaption>
    </figure>
    <div class="media-text">
      <ul>
        <li><strong>Problem:</strong> Design and build a functional C-clamp from concept to tested prototype within strict manufacturing constraints.</li>
        <li><strong>Role:</strong> Team of 2 (co-designed, modeled, fabricated, and tested).</li>
        <li><strong>Tools:</strong> SolidWorks CAD/CAM, CNC milling, FDM 3D printing (Bambu Lab slicer).</li>
        <li><strong>Status:</strong> Prototype built and tested.</li>
      </ul>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>The Engineering Problem</h3>
  <ul>
    <li><strong>Goal:</strong> Produce a clamp that reliably applies and holds load within course manufacturing rules.</li>
    <li><strong>Parts required:</strong></li>
  </ul>
  <ul>
    <li>C-shaped frame CNC-machined from PVC</li>
    <li>Threaded screw with swivel pad (3D printed)</li>
    <li>Threaded portion of the frame (3D printed)</li>
  </ul>
  <ul>
    <li><strong>No adhesives:</strong> Joint strength must come from geometry and tolerances.</li>
    <li><strong>FDM limits:</strong> Thread quality forced print orientations that weren’t ideal for joint strength.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Our Approach</h3>
  <div class="media-block media-right">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/frame_drawing.png' | relative_url }}" alt="C-frame technical drawing">
      <figcaption class="tagline">Technical drawing of the CNC-machined C-frame.</figcaption>
    </figure>
    <div class="media-text">
      <ul>
        <li><strong>Joint strategy:</strong> Dovetail interface between printed insert and CNC frame to resist pullout and torsion without adhesives.</li>
        <li><strong>Tradeoff:</strong> Tighter tolerances improve mechanical lock but are harder to hit across CNC + FDM parts.</li>
      </ul>
    </div>
  </div>
  <div class="media-block media-left">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/foot_drawing.png' | relative_url }}" alt="Clamp foot technical drawing">
      <figcaption class="tagline">Clamp foot drawing highlighting the swivel contact geometry.</figcaption>
    </figure>
    <div class="media-text">
      <ul>
        <li><strong>Contact design:</strong> Ball-and-socket swivel pad to self-align and reduce point loading.</li>
        <li><strong>Iteration:</strong> Multiple print trials to balance snap-fit ease, pull-off resistance, and rotation.</li>
      </ul>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>Analysis &amp; Calculations</h3>
  <ul>
    <li><strong>Critical load path:</strong> Dovetail joint + printed insert expected to govern failure under high clamp force.</li>
    <li><strong>Observed mode:</strong> Printed insert deformation at the dovetail during overload, indicating thin section and print-orientation weakness.</li>
  </ul>
</section>

<section class="section-card">
  <h3>CAD, Drawings &amp; Manufacturing</h3>
  <div class="media-block media-right">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/3d_print.png' | relative_url }}" alt="3D-printed clamp components">
      <figcaption class="tagline">All 3D-printed components before assembly.</figcaption>
    </figure>
    <div class="media-text">
      <ul>
        <li><strong>CAD/CAM:</strong> SolidWorks design; SolidWorks CAM for CNC toolpaths.</li>
        <li><strong>3D printing:</strong> Bambu Lab slicer for printed components.</li>
        <li><strong>Drawings:</strong> Fully dimensioned prints used to verify CNC frame accuracy.</li>
      </ul>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>Testing, Validation &amp; Results</h3>
  <ul>
    <li><strong>Performance:</strong> Held 5 kg without slip; failed at 7 kg.</li>
    <li><strong>Failure location:</strong> Dovetail joint at the printed insert.</li>
    <li><strong>Root cause:</strong> Thin section + FDM layer behavior + joint orientation allowed rotation under load.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Outcomes &amp; Impact</h3>
  <ul>
    <li><strong>Requirement met:</strong> Held 5 kg and validated a full concept-to-test build under the required constraints.</li>
    <li><strong>Clear redesign target:</strong> Dovetail/insert geometry governed failure at 7 kg.</li>
  </ul>
</section>

<section class="section-card">
  <h3>What I Learned</h3>
  <ul>
    <li><strong>CNC workflow:</strong> Planning and verification matter as much as machining time.</li>
    <li><strong>FDM reality:</strong> Orientation and tolerances drive both strength and fit; multiple reprints were required.</li>
    <li><strong>Design insight:</strong> Joint design and load paths dominate performance; failure analysis shaped redesign thinking.</li>
  </ul>
</section>

<section class="section-card">
  <h3>What I’d Improve Next</h3>
  <ul>
    <li>Push more of the load into the CNC-machined PVC frame instead of the 3D-printed insert.</li>
    <li>Increase the cross-sectional thickness of the printed joint.</li>
    <li>Reorient the joint geometry so it better resists the loading from tightening the screw.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Skills Highlight</h3>
  <ul>
    <li>Mechanical design</li>
    <li>Solid mechanics</li>
    <li>CAD (SolidWorks)</li>
    <li>CNC planning and machining</li>
    <li>FDM 3D printing</li>
    <li>Design for Manufacturing &amp; Assembly (DFM/DFA)</li>
    <li>Failure analysis</li>
  </ul>
</section>
