---
title: "Bugs and the ALS"
description: ""
---

<div class="slide slide-1">
  <div class="slide-1-left">
    <p>I had the opportunity to work at the Advanced Light Source (ALS) at Berkeley Lab — a synchrotron particle accelerator — where I worked on Beamline 8.3.2, which specializes in X-ray micro-computed tomography (micro-CT).</p>
    <p>Tomography involves using X-rays to image the internal structure of objects within a field of view of</p>
    <img class="slide-1-building" src="/images/project1/als-dome.jpg" alt="The Advanced Light Source dome building at Berkeley Lab">
  </div>
  <div class="slide-1-right">
    <img src="/images/project1/hallway.jpg" alt="Entrance to the ALS experiment floor">
    <img src="/images/project1/objectives.jpg" alt="Microscope objective lenses on the imaging rig">
  </div>
</div>

<div class="slide slide-2">
  <div class="slide-2-left">
    <p>Studying Bugs for its fascinating Biomechanics!</p>
    <p>I worked with Sharpshooters a bug which uses "super propulsion" to flick pee at accelerations exceeding 40 g's about the acceleration of 40 cheetahs.</p>
    <p>I worked with Prof. Jacob Harrison of Morehouse College to build 3D models of the sharpshooter at three life stages young, middle, and mature tracing how its Flicker develops over time. Studying how that limb functions gives techniques to apply to robotics.</p>
    <p>With the use of the particle accelerator I am able to create scans to examine these incredibly small structures!</p>
  </div>
  <div class="slide-2-right">
    <div class="slide-2-pair">
      <img src="/images/project1/scan-pyramid.jpg" alt="3D scan reconstruction of an insect part, pyramid-like structure">
      <img class="slide-2-inset" src="/images/project1/scan-closeup.jpg" alt="Close-up detail of the 3D scan reconstruction">
    </div>
    <div class="slide-2-pair">
      <img src="/images/project1/scan-cone.jpg" alt="3D scan reconstruction with fine bristle detail">
      <img class="slide-2-inset" src="/images/project1/scan-mouth.jpg" alt="Close-up detail of mouthpart structures">
    </div>
  </div>
  <img class="slide-2-peek" src="/images/project1/leafhopper.jpg" alt="A leafhopper and nymph on a plant stem">
</div>

<div class="slide slide-3">
  <div class="slide-3-left">
    <p>How were these Created?</p>
    <p>The first thing on our agenda was collecting all the bugs that we wanted to research and scan using the beamline.</p>
    <p>We did this by visiting the Essig Museum of Entomology Research at UC Berkeley to borrow some of the specimen.</p>
    <p>Here are some pictures of our visit!</p>
  </div>
  <div class="slide-3-right">
    <img class="slide-3-round" src="/images/project1/group-drawer.jpg" alt="Group looking at a drawer of pinned insect specimens">
    <img src="/images/project1/specimen-hemiptera.jpg" alt="Hemiptera specimen under magnification, 1mm scale">
    <img src="/images/project1/collection-cabinet.jpg" alt="Opening a specimen drawer in the insect collection cabinets">
    <img src="/images/project1/specimen-grasshopper.jpg" alt="Grasshopper specimen under magnification, 2mm scale">
  </div>
</div>

<div class="slide slide-4">
  <div class="slide-4-images">
    <img class="s4-a" src="/images/project1/dragonfly-segment.jpg" alt="Dragonfly software segmenting an insect scan in cross-section">
    <img class="s4-b" src="/images/project1/chuck-mount.jpg" alt="A specimen mounted in a chuck at the imaging setup">
    <img class="s4-c" src="/images/project1/desk-dual-monitor.jpg" alt="Workstation with dual monitors used for scan analysis">
    <img class="s4-d" src="/images/project1/render-dark.jpg" alt="3D render of a scanned specimen in modeling software">
  </div>
  <div class="slide-4-right">
    <ul>
      <li>The dead specimens were first scanned using a synchrotron beamline.</li>
      <li>I transferred and combined the scan's layered slices into a full 3D volume using Dragonfly software.</li>
      <li>I used MeshLab to verify that every part of the body was captured in the mesh.</li>
      <li>Then I used Blender to make up every other body part that was lost during scanning</li>
      <li>I used Fusion 360 to
        <ul>
          <li>Convert the organic mesh into a precise solid model for measurement/analysis</li>
          <li>Compare dimensions/scale across the three life stages</li>
          <li>Clean up and prep the final files for 3D printing physical models</li>
        </ul>
      </li>
    </ul>
  </div>
</div>
