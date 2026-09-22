---
title: "Vehicle Dynamics Research Project"
description: ""
url: /vehicle-dynamics/
---

<div class="slide">
  <p>I was really interested in the dynamics of formula cars and how they worked, so I decided to take on a research project on tire dynamics. Understanding how tires work is something I want to apply toward building my own car someday, and maybe even racing it.</p>
  <p>The first thing I did was dig into the technical requirements and existing research on tire behavior. I also wanted to make sure I understood the parts that control the tires like the suspension and the parts that make it up.</p>
</div>

<div class="slide slide-2col">
  <div>
    <p><strong>What is the minimum wheelbase value allowed?</strong><br>- 1525mm</p>
    <p><strong>What is the minimum usable wheel travel value with a driver seated?</strong><br>- 50mm</p>
    <p><strong>What type of fasteners must be used in the suspension and steering systems?</strong><br>- Critical Fasteners<br>&nbsp;&nbsp;- bolts, nuts, and screws</p>
    <p><strong>Should spherical rod ends and spherical bearings be mounted in single shear or double shear?</strong><br>- Double shear</p>
    <p><strong>What is the minimum wheel size allowed?</strong><br>- 203.2 mm (8.0 inches) or more in diameter.</p>
  </div>
  <div>
    <p><strong>What are the 3 minimum critical fastener specifications that must be met?</strong><br>- SAE Grade 5, Metric Class 8.8, AN/MS Specifications</p>
    <p><strong>How should critical fasteners be secured from unintentional loosening?</strong><br>- not be countersunk, Technical Inspectors, Do not rely on the clamping force, locking device</p>
    <p><strong>What is the minimum number of full threads that must project from any lock nut?</strong><br>- Two full threads</p>
  </div>
</div>

<div class="slide slide-2col">
  <div>
    <p><strong>Physics of Racing:</strong><br>Yaw &amp; Polar Moment of Inertia</p>
    <ul>
      <li>Pull the heavy stuff in toward the center, shrink the polar moment of inertia, makes car easier to turn/move.</li>
    </ul>
    <p><strong>Key Components:</strong></p>
    <ul>
      <li>Lower and Upper control arms &ndash; Helps connect the Upright to the Chassis</li>
      <li>Upright &ndash; Central mounting point, holds things together</li>
      <li>Tie rod &ndash; What turns the wheel when steering</li>
      <li>Rod ends/spherical bearings &ndash; Lets the arms and tie rod pivot freely</li>
      <li>Pushrod / pullrod &ndash; Moves the up and down motion to Rocker</li>
    </ul>
  </div>
  <div>
    <p><strong>Key components:</strong></p>
    <ul>
      <li>Rocker &ndash; Middle man, moves vertical motion to spring/damper away from wheel</li>
      <li>Spring &ndash; Supports load, resists compression</li>
      <li>Damper &ndash; Dissipates unwanted vertical energy</li>
      <li>Wheel Bearing &ndash; Lets wheel/hub spin freely relative to upright</li>
      <li>Hub &ndash; What the wheel bolts to, rotates</li>
      <li>Anti-roll bar &ndash; Connects left and right suspension to resist body roll</li>
      <li>Brake Disc &ndash; Pins with the wheel/hub and spins</li>
      <li>Brake Caliper &ndash; Clamps brake disc to slow the wheel down when braking</li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/graph-fy-alpha.png" alt="Lateral force vs slip angle graph, Blue 2kN, Red 4kN, Yellow 6kN, Purple 8kN">
  <div>
    <p><strong>Lateral force vs slip angle</strong><br>Blue: 2kN, Red: 4kN, Yellow: 6kN, Purple: 8kN</p>
    <p><strong>The graph observation:</strong></p>
    <ul>
      <li>As slip angle increases in magnitude so does the lateral force
        <ul>
          <li>Until a certain alpha where it curves then flattens and finally declines a little</li>
          <li>That curve shifts wider with a heavier load</li>
          <li>A larger load can handle more slip angle before the tire starts to slip</li>
        </ul>
      </li>
    </ul>
    <p><strong>The vehicle design:</strong></p>
    <ul>
      <li>We know the more load the more lateral force we can produce
        <ul>
          <li>BUT we also know F = ma</li>
          <li>The graph is non linear and curves down</li>
          <li>Extra force from more load does not make up for the mass</li>
          <li>The more load the less acceleration</li>
        </ul>
      </li>
      <li>Race car so we want something that can make sharp turns
        <ul>
          <li>Make it as light as we can</li>
        </ul>
      </li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/graph-bcd-fz.png" alt="Cornering stiffness BCD vs vertical load Fz graph">
  <div>
    <p><strong>Cornering Stiffness vs Lateral Force</strong></p>
    <p><strong>The graph observation:</strong></p>
    <ul>
      <li>BCD climbs up to peak around ~5.6-5.7 and declines from there to 8kN</li>
      <li>Now we know that more load doesn't always mean the tires produce more grip/Fy</li>
      <li>The decline means the tire's responsiveness isn't keeping pace with load anymore</li>
    </ul>
    <p><strong>Load transfer:</strong></p>
    <ul>
      <li>Since BCD differs by load outer and inner tires have different values
        <ul><li>Each tire contributes a different force</li></ul>
      </li>
      <li>Curve is non linear so the loss of force is greater than the gain
        <ul><li>Net total loss of grip on axle</li></ul>
      </li>
    </ul>
    <p><strong>The vehicle design:</strong></p>
    <ul>
      <li>Don't want a large BCD since possibility tires are too responsive and slip by accident</li>
      <li>Large enough to respond quick to turn?</li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/graph-d-fz.png" alt="Peak lateral force D vs vertical load Fz graph">
  <div>
    <p><strong>Cornering Stiffness vs Lateral Force</strong></p>
    <p><strong>The graph observation:</strong></p>
    <ul>
      <li>As load increases the peak lateral force does too</li>
      <li>Not linear, curves downward</li>
    </ul>
    <p><strong>Load transfer:</strong></p>
    <ul>
      <li>Graph nonlinear so in load transfer D is not exchanged equally
        <ul>
          <li>The outer tires gain is smaller than the loss of the inner tires</li>
          <li>The maximum total traction decreases with a turn</li>
        </ul>
      </li>
      <li>The larger the transfer the bigger the decrease in D, minimal transfer does not affect traction as much.</li>
    </ul>
    <p><strong>The vehicle design:</strong></p>
    <ul>
      <li>Want sharper turns we would stiffen the rear ARB
        <ul><li>Oversteer possible *</li></ul>
      </li>
      <li>Would sacrifice more stability</li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <div class="slide-sideimg-imgs cols-2">
    <img src="/images/vehicle-dynamics/code-calcmaxfy.png" alt="calc_max_fy.m MATLAB function code">
    <img src="/images/vehicle-dynamics/code-fymax.png" alt="F_y_max.m MATLAB function code">
  </div>
  <div>
    <p><strong>Calc_max_fy and F_y_max function</strong></p>
    <p><strong>Purpose:</strong><br>We need a function that can calculate the Fy when there is a load transfer.</p>
    <p>A helper function for another function to calculate Fymax</p>
    <ul>
      <li>Same Thing is calculated for the inner</li>
      <li>Calculates Fy by adding both inner Fy and outer</li>
      <li>Negative since we use fminsearch
        <ul><li>It searches for the min</li></ul>
      </li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <div class="slide-sideimg-imgs">
    <img src="/images/vehicle-dynamics/code-calcfy.png" alt="calc_Fy.m MATLAB function code">
    <img src="/images/vehicle-dynamics/code-getalpha.png" alt="get_alpha.m MATLAB function code">
  </div>
  <div>
    <p><strong>calc_Fy and get_alpha function</strong></p>
    <p><strong>Purpose for calc_Fy:</strong><br>Created to get the Fy of a Fzi, Fzo and subtract it from a desired Fy</p>
    <p>This is to see the difference</p>
    <p>Helper function</p>
    <p><strong>Purpose for get_alpha:</strong><br>Function returns an alpha to a desired Fy</p>
    <p>We are starting the guess at 1, I just chose it because its 1 its the beginning</p>
    <p>fsolve calls calc_Fy repeatedly until it finds a alpha/slip angle that satisfies the desired Fy leaving no difference</p>
  </div>
</div>

<div class="slide slide-sideimg">
  <div class="slide-sideimg-imgs">
    <img src="/images/vehicle-dynamics/code-test-script.png" alt="Testing script for F_y_max and get_alpha functions">
    <img src="/images/vehicle-dynamics/graph-test-fy.png" alt="Fy,tot vs alpha test graph with Fymax and Fy_desired marked">
  </div>
  <div>
    <p><strong>Testing F_y_max and get_alpha functions</strong></p>
    <p><strong>Purpose:</strong></p>
    <ul>
      <li>Testing both functions</li>
      <li>Want for bicycle model</li>
      <li>Draws a Fy vs alpha graph</li>
      <li>Marks where Fymax is and the slip angle for the specific Fy we wanted
        <ul><li>That being 3000N</li></ul>
      </li>
      <li>Chose Fzi = 2kN, Fzo = 6kN</li>
      <li>Graph shows they work
        <ul><li>Ready for the bicycle model</li></ul>
      </li>
    </ul>
  </div>
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/code-variables.png" alt="MATLAB code collecting the flowchart variables">
  <div>
    <p>Collecting the variables that we'll need to go through the flowchart</p>
    <img src="/images/vehicle-dynamics/flowchart.png" alt="Flowchart: calculate lateral acceleration, lateral tire forces, roll angle, normal load on all 4 tires, peak lateral force, slip angles, steering angle" style="width:100%; margin-top:16px; border-radius:var(--radius); border:1px solid var(--border); background:#fff;">
  </div>
</div>

<div class="slide slide-shot cols-1">
  <img src="/images/vehicle-dynamics/code-forloop-left.png" alt="MATLAB for loop code, load transfer and peak force calculations">
</div>
<div class="slide slide-shot cols-1">
  <img src="/images/vehicle-dynamics/code-forloop-right.png" alt="MATLAB for loop code, feasibility check and steering angle calculation">
</div>

<div class="slide">
  <p>plotting!</p>
  <img src="/images/vehicle-dynamics/code-plotting.png" alt="MATLAB plotting code for slip angle and steering angle graphs" style="width:100%; margin-top:16px; border-radius:var(--radius); border:1px solid var(--border); background:#fff;">
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/graph-slip-baseline.png" alt="Front vs Rear Slip Angle graph, blue front, red rear, understeer">
  <div>
    <p>Blue is front, Red is rear</p>
    <p>Based on the car's design variables and the tested velocity range, this car understeers meaning the front axle reaches its slip limit first.</p>
    <p>Stiffening the rear ARB would shift more load transfer to the rear, narrowing this gap and pushing the balance toward oversteer.</p>
    <p>Or I could even try to balance the weight a little more so the moment of inertia is more in the middle</p>
  </div>
</div>

<div class="slide slide-sideimg">
  <img src="/images/vehicle-dynamics/graph-steering-baseline.png" alt="Required steering angle vs velocity graph">
  <div>
    <p><strong>Steering angle vs Velocity graph</strong></p>
    <p>Boom! This is the graph that shows the calculated steering angles for any level of lateral acceleration</p>
    <p>This is because lateral acceleration only changes when V changes since the radius is a constant 15 m. Acc = V^2 / R</p>
    <p>Here you can see that as velocity increases so does the need for the tires to be steered at a larger angle</p>
    <p>You can see around 10.5 there's bigger jumps</p>
    <p>I would attribute this to the tires starting to get close to slipping and needing that extra push to stay on track</p>
  </div>
</div>

<div class="slide slide-sideimg">
  <div class="slide-sideimg-imgs">
    <img src="/images/vehicle-dynamics/graph-slip-oversteer.png" alt="Front vs Rear Slip Angle graph after increasing rear roll stiffness, rear now exceeds front">
    <img src="/images/vehicle-dynamics/graph-steering-oversteer.png" alt="Required steering angle vs velocity graph after increasing rear roll stiffness">
  </div>
  <div>
    <img src="/images/vehicle-dynamics/code-vars-oversteer.png" alt="MATLAB variables with Kr_spring changed to 350" style="width:100%; margin-bottom:16px; border-radius:var(--radius); border:1px solid var(--border); background:#fff;">
    <p>Changed the Kr_spring/ rear roll stiffness from 250 to 350</p>
    <p>It slipped to oversteer!</p>
    <p>We can see the steering angle vs velocity graph</p>
    <p>&lt;- Steep curve is due to the rear angle growing more than front</p>
  </div>
</div>

<div class="slide slide-sideimg">
  <div class="slide-sideimg-imgs">
    <img src="/images/vehicle-dynamics/graph-slip-cg.png" alt="Front vs Rear Slip Angle graph after balancing the CG, front wheels slip">
    <img src="/images/vehicle-dynamics/graph-steering-cg.png" alt="Required steering angle vs velocity graph after balancing the CG">
  </div>
  <div>
    <img src="/images/vehicle-dynamics/code-vars-cg.png" alt="MATLAB variables with CG distances a and b both set to 1.29" style="width:100%; margin-bottom:16px; border-radius:var(--radius); border:1px solid var(--border); background:#fff;">
    <p>Another where we changed the CG of a and b from 1.16, 1.42 respectively to 1.29 each to make the weight distribution equal!</p>
    <p>Wow the front wheels slipped!</p>
    <p>Im assuming its because of the uneven roll stiffness!</p>
    <p>&lt;- Rear angle growing more than front</p>
  </div>
</div>
