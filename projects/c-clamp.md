---
layout: default
title: C-Clamp
---

<section class="section-card">
  <h2>C-Clamp Manufacturing Project</h2>
  <h3>Description</h3>
  <div class="media-block media-left">
    <figure class="media-figure media-figure-small media-figure-rotate-left">
      <img src="{{ '/assets/projects/c-clamp/full.png' | relative_url }}" alt="Full C-clamp assembly">
      <figcaption class="tagline">Full assembly of the C-clamp after fabrication and testing.</figcaption>
    </figure>
    <div class="media-text">
      <p>For a manufacturing processes course, my partner and I designed and built a functional C-clamp from scratch. The goal was to take a simple mechanical tool all the way from concept to a finished, tested part, while working within a set of manufacturing constraints that heavily influenced the final design. Along the way, I learned about DFM, DFA, working with CAM software and 3D printing.</p>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>Project Scope &amp; Constraints</h3>
  <p>The clamp had to be made from three separate parts:</p>
  <ul>
    <li>A C-shaped frame CNC-machined from PVC</li>
    <li>A threaded screw with a swivel pad, manufactured using 3D printing</li>
    <li>The threaded portion of the frame, also 3D printed</li>
  </ul>
  <p>On top of that, we weren’t allowed to use any adhesives to connect the threaded insert to the rest of the frame. This meant we had to rely entirely on geometry and tolerances to create a joint that could handle the forces involved in clamping.</p>
  <p>At the same time, we had to work around the limitations of FDM 3D printing, especially when it came to printing usable threads. In practice, this locked us into certain print orientations to get clean threads, even if those orientations weren’t ideal for the strength or geometry of the joint.</p>
</section>

<section class="section-card">
  <h3>Design Rationale</h3>
  <div class="media-block media-right">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/frame_drawing.png' | relative_url }}" alt="C-frame technical drawing">
      <figcaption class="tagline">Technical drawing of the CNC-machined C-frame.</figcaption>
    </figure>
    <div class="media-text">
      <p>To connect the 3D-printed threaded insert to the CNC-machined frame, we went with a dovetail joint, taking inspiration from woodworking. The idea was that with tight enough tolerances, the dovetail would provide a strong mechanical lock without needing glue or fasteners. This pushed us to think carefully about what tolerances were actually achievable when mixing CNC machining and FDM printing.</p>
    </div>
  </div>
  <div class="media-block media-left">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/foot_drawing.png' | relative_url }}" alt="Clamp foot technical drawing">
      <figcaption class="tagline">Clamp foot drawing highlighting the swivel contact geometry.</figcaption>
    </figure>
    <div class="media-text">
      <p>We also realized early on that the threaded screw needed to be separate from the swivel pad that contacts the workpiece. Having a rotating pad allows the clamp to sit better on uneven or non-flat surfaces and reduces point loading. To make this work, we designed a ball-and-socket joint between the screw and the swivel pad.</p>
      <p>Getting this joint right took a few iterations. The fit needed to be loose enough that the pad could be snapped on by hand and rotate freely, but tight enough that it wouldn’t pull off under load. We printed and tested multiple versions until we found a balance that met those goals.</p>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>Manufacturing Process</h3>
  <div class="media-block media-right">
    <figure class="media-figure">
      <img src="{{ '/assets/projects/c-clamp/3d_print.png' | relative_url }}" alt="3D-printed clamp components">
      <figcaption class="tagline">All 3D-printed components before assembly.</figcaption>
    </figure>
    <div class="media-text">
  <p>All of the parts were designed in SolidWorks. We generated CNC toolpaths for the frame using SolidWorks’ built-in CAM tools, and planned all of the 3D-printed parts using Bambu Lab’s slicing software.</p>
      <p>We also created fully dimensioned technical drawings for each part and used them to check the accuracy of the CNC-machined frame. This was a good reminder that even when you design everything in CAD, the real world always introduces some variation.</p>
    </div>
  </div>
</section>

<section class="section-card">
  <h3>Testing &amp; Performance</h3>
  <p>The final clamp ended up being heavier than many others in the class, but it performed well. It was able to support a 5 kg load without slipping or breaking, and ultimately failed at 7 kg.</p>
  <p>The failure happened at the dovetail joint, where the 3D-printed insert began to deform. The geometry in that region was too thin, and the layered nature of FDM printing made the part fairly ductile. On top of that, the orientation of the dovetail allowed the insert to rotate slightly as the clamping force from the threaded screw and swivel pad increased, which sped up the failure.</p>
</section>

<section class="section-card">
  <h3>Key Learnings</h3>
  <p>This project was my first real hands-on experience using a CNC mill in an academic setting. I had done manual machining in high school robotics, but working with CNC added a new layer of planning and verification that I hadn’t dealt with before.</p>
  <p>I also gained a much better feel for FDM 3D printing, especially how print orientation, geometry, and printer settings affect both strength and dimensional accuracy. We had to reprint several parts because they didn’t fit quite right, which made the impact of tolerances very real.</p>
  <p>From a design perspective, the project really highlighted how important joint design and load paths are. The failure analysis was just as valuable as the successful parts, and it gave me a clearer idea of how I would approach a redesign.</p>
</section>

<section class="section-card">
  <h3>Future Improvements</h3>
  <ul>
    <li>Push more of the load into the CNC-machined PVC frame instead of the 3D-printed insert.</li>
    <li>Increase the cross-sectional thickness of the printed joint.</li>
    <li>Reorient the joint geometry so it better resists the loading from tightening the screw.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Tools &amp; Skills Used</h3>
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
