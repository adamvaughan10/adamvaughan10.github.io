---
layout: default
title: C-Clamp
---

<section class="section-card">
  <h2>C-Clamp Design &amp; Manufacturing Project</h2>
  <p class="tagline">Designed and manufactured a functional C-clamp under strict constraints, integrating CNC machining, 3D printing, CAD, and tolerance analysis.</p>
</section>

<section class="section-card">
  <h3>Overview</h3>
  <p>As part of a Manufacturing Processes course, I designed and manufactured a functional C-clamp from concept through fabrication. The project required integrating CNC machining, additive manufacturing, CAD, and tolerance analysis while working under strict design constraints that forced deliberate engineering tradeoffs.</p>
  <p>The final clamp successfully supported a 5 kg load without slippage or fracture, with failure occurring at 7 kg, providing a valuable opportunity for failure analysis and design iteration.</p>
  <figure class="project-figure">
    <img src="{{ '/assets/projects/c-clamp/full.png' | relative_url }}" alt="Full C-clamp assembly">
    <figcaption class="tagline">Full assembly of the C-clamp after fabrication and testing.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Project Requirements &amp; Constraints</h3>
  <ul>
    <li>Clamp composed of three distinct parts: C-shaped frame (CNC-machined from PVC), screw (3D printed), and threaded insert section of the frame (3D printed).</li>
    <li>No adhesives permitted to join the threaded insert to the frame.</li>
    <li>Threads had to be fully functional despite 3D-printing limitations.</li>
    <li>Required submission of technical drawings and dimensional verification against manufactured parts.</li>
  </ul>
  <p>These constraints strongly influenced material selection, joint design, and manufacturing strategy.</p>
</section>

<section class="section-card">
  <h3>Design Rationale &amp; Engineering Decisions</h3>
  <h4>Frame–Threaded Insert Interface</h4>
  <p>To connect the 3D-printed threaded insert to the CNC-machined frame without adhesives, we designed a tight-tolerance dovetail joint inspired by woodworking joinery.</p>
  <p>Engineering considerations included load transfer from the screw into the frame, stress concentration at the joint interface, print-orientation limitations of the threaded geometry, and achievable tolerances for CNC vs. FDM printing. The dovetail allowed for mechanical interlock while avoiding secondary fastening methods.</p>
  <figure class="project-figure">
    <img src="{{ '/assets/projects/c-clamp/frame_drawing.png' | relative_url }}" alt="C-frame technical drawing">
    <figcaption class="tagline">Technical drawing of the CNC-machined C-frame.</figcaption>
  </figure>
  <h4>Screw &amp; Swivel Foot Design</h4>
  <p>To improve real-world usability, the clamp incorporated a rotating contact foot to accommodate non-flat surfaces.</p>
  <p>This required separating the screw shaft from the contact foot and designing a ball-and-socket joint that allowed free rotation while resisting pull-out. Multiple print iterations were tested to balance ease of assembly, retention force, and durability under repeated loading.</p>
  <figure class="project-figure">
    <img src="{{ '/assets/projects/c-clamp/foot_drawing.png' | relative_url }}" alt="Clamp foot technical drawing">
    <figcaption class="tagline">Clamp foot drawing highlighting the swivel contact geometry.</figcaption>
  </figure>
  <figure class="project-figure">
    <video controls playsinline>
      <source src="{{ '/assets/projects/c-clamp/ball_and_socket.mov' | relative_url }}" type="video/quicktime">
    </video>
    <figcaption class="tagline">Ball-and-socket joint motion test for the swivel foot.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Manufacturing Workflow</h3>
  <h4>CAD &amp; CAM</h4>
  <ul>
    <li>All components modeled in SolidWorks.</li>
    <li>CNC toolpaths generated using SolidWorks CAM.</li>
    <li>Fully dimensioned technical drawings created for each part.</li>
  </ul>
  <h4>CNC Machining</h4>
  <ul>
    <li>Machined the C-frame from PVC using a CNC mill.</li>
    <li>Used drawings to verify dimensional accuracy, surface finish, and fit with 3D-printed components.</li>
  </ul>
  <h4>Additive Manufacturing</h4>
  <ul>
    <li>Printed threaded components and screw using FDM.</li>
    <li>Planned prints in Bambu Lab slicing software.</li>
    <li>Adjusted print orientation, layer height, infill, and wall thickness to balance strength, accuracy, and print success.</li>
  </ul>
  <figure class="project-figure">
    <img src="{{ '/assets/projects/c-clamp/3d_print.png' | relative_url }}" alt="3D-printed clamp components">
    <figcaption class="tagline">All 3D-printed components before assembly.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Testing &amp; Failure Analysis</h3>
  <ul>
    <li>Successfully supported 5 kg without deformation or slip.</li>
    <li>Failed at 7 kg, with failure localized to the dovetail joint.</li>
  </ul>
  <p>Failure mode analysis showed plastic deformation of thin 3D-printed dovetail geometry. Layer-based construction allowed shear and rotation under increasing screw load, and joint orientation was not optimally aligned with applied loading. This provided direct insight into anisotropy and ductility in FDM-printed parts.</p>
</section>

<section class="section-card">
  <h3>Key Learnings</h3>
  <h4>Mechanical &amp; Structural</h4>
  <ul>
    <li>Practical effects of tolerances across mixed manufacturing methods.</li>
    <li>Load paths and stress concentrations in mechanical joints.</li>
    <li>Importance of aligning joint geometry with expected loading.</li>
    <li>Material behavior differences between homogeneous stock and layered prints.</li>
  </ul>
  <h4>Manufacturing</h4>
  <ul>
    <li>First hands-on experience running a CNC mill in an academic setting.</li>
    <li>Tradeoffs between print orientation and dimensional accuracy.</li>
    <li>Iterative prototyping as a core engineering tool.</li>
  </ul>
  <h4>Design Process</h4>
  <ul>
    <li>Designing under real constraints forces better engineering decisions.</li>
    <li>Early prototyping can significantly reduce downstream failures.</li>
    <li>Failure analysis is as valuable as success in improving designs.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Skills &amp; Tools Used</h3>
  <h4>Engineering Skills</h4>
  <ul>
    <li>Mechanical design</li>
    <li>Solid mechanics</li>
    <li>Tolerance analysis</li>
    <li>Failure analysis</li>
    <li>Design for Manufacturing &amp; Assembly (DFM/DFA)</li>
  </ul>
  <h4>Software &amp; Tools</h4>
  <ul>
    <li>SolidWorks (CAD, CAM, technical drawings)</li>
    <li>CNC milling</li>
    <li>FDM 3D printing</li>
    <li>Bambu Lab slicing software</li>
  </ul>
  <h4>Processes</h4>
  <ul>
    <li>CNC planning and verification</li>
    <li>Rapid prototyping</li>
    <li>Iterative design validation</li>
  </ul>
</section>

<section class="section-card">
  <h3>Future Improvements</h3>
  <ul>
    <li>Redesign the joint to shift more load into the CNC-machined PVC frame.</li>
    <li>Increase cross-sectional thickness of the 3D-printed dovetail.</li>
    <li>Reorient the joint to oppose applied screw torque.</li>
    <li>Prototype multiple joint concepts earlier in the design cycle.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Project Outcomes</h3>
  <ul>
    <li>Functional clamp meeting all project requirements.</li>
    <li>Load capacity competitive within the class.</li>
    <li>Strong practical understanding of manufacturing-driven design constraints.</li>
    <li>Clear linkage between analysis, fabrication, testing, and redesign.</li>
  </ul>
</section>
