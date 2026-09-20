---
title: "Berkeley Lab, Biomechanics Research Intern"
description: ""
url: /LBNL2/
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

<div class="slide slide-textphotos">
  <div class="slide-textphotos-text">
    <p>Here are videos comparing the size of young and mature sharpshooters.</p>
    <p>The young one is on the left and the mature one is on the right. A young sharpshooters tip of the tail grows into the massive flicker we see on the right</p>
  </div>
  <div class="slide-textphotos-images slide-videos">
    <img src="/images/project1/video-compare-both.webp" alt="Video comparing the young and mature sharpshooter tail side by side">
    <img src="/images/project1/video-mature-solo.webp" alt="Video of the mature sharpshooter tail scan rotating">
  </div>
</div>

<div class="slide slide-textphotos">
  <div class="slide-textphotos-text">
    <p>Here are scans comparing the internal structure of a young and a mature flicker.</p>
    <p>Watch how the tiny limb changes as the sharpshooter grows, and you can see how it builds up to launching droplets at over 40 g.</p>
    <p>The one on the right is the late stage and the left is the early stages</p>
  </div>
  <div class="slide-textphotos-images slide-videos">
    <img src="/images/project1/video-internal-young.webp" alt="Internal CT scan video of the young sharpshooter">
    <img src="/images/project1/video-internal-mature.webp" alt="Internal CT scan video of the mature sharpshooter">
  </div>
</div>

<div class="slide slide-textphotos">
  <div class="slide-textphotos-text">
    <p>How were these Created?</p>
    <p>The first thing on our agenda was collecting all the bugs that we wanted to research and scan using the beamline.</p>
    <p>We did this by visiting the Essig Museum of Entomology Research at UC Berkeley to borrow some of the specimen. Here are some pictures of our visit!</p>
  </div>
  <div class="slide-textphotos-images">
    <img src="/images/project1/essig-drawer2.jpg" alt="Group looking at a specimen drawer at the Essig Museum">
    <img src="/images/project1/essig-monitor.jpg" alt="Group examining a specimen on a microscope monitor">
    <img src="/images/project1/essig-tray-hold.jpg" alt="Curator holding a specimen tray in the museum cabinet aisle">
  </div>
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

<div class="slide slide-5">
  <div class="slide-5-images">
    <img src="/images/project1/maya-ladybug.jpg" alt="A ladybug model being animated in Maya">
    <img src="/images/project1/vr-museum.jpg" alt="A virtual museum room hosting 3D modeled bugs on pedestals">
    <img src="/images/project1/vr-headsets.jpg" alt="Two people trying the VR bug museum with headsets on">
    <img src="/images/project1/vr-desk.jpg" alt="Viewing the VR experience on a monitor at a desk">
  </div>
  <div class="slide-5-right">
    <p>From there we started our journey to make learning about our bug research into a VR experience</p>
    <p>We did this by</p>
    <ul>
      <li>Working with Maya a animation software so that we could make animations of the models to use in VR</li>
      <li>We also used blender to for other bugs we wanted to showcase</li>
      <li>Then from there we had everything we needed to transfer our things to VR</li>
      <li>We used Sketchfab to host our museum of 3D modeled bugs!</li>
    </ul>
  </div>
</div>

<div class="slide slide-textphotos">
  <div class="slide-textphotos-text">
    <p>And from there we had our presentation during cookie time. Cookie time being a tradition where the ALS every thursday has cookies and coffee outside the building to make people get together and catch up.</p>
    <p>This is where we talked and showcased our project to the ALS faculty of what we did over the summer!</p>
  </div>
  <div class="slide-textphotos-images">
    <img src="/images/project1/cookie-booth.jpg" alt="Kids trying VR headsets at the Discover the World of Bugs booth">
    <img src="/images/project1/cookie-crowd.jpg" alt="A crowd gathered at the ALS lobby during cookie time">
  </div>
</div>

<div class="slide slide-textphotos">
  <div class="slide-textphotos-text">
    <p>We also got invited to present our research at a conference!</p>
    <p>We did this at a doubletree at the Berkeley Marina in front of faculty of the ALS and some other parts of the country that use all sorts of particle accelerators!</p>
  </div>
  <div class="slide-textphotos-images">
    <img src="/images/project1/present-mic.jpg" alt="Presenting the sharpshooter research with a microphone at the conference">
    <img src="/images/project1/conference-selfie.jpg" alt="Group selfie with fellow researchers at the conference table">
  </div>
</div>
