---
layout: page
title: F1-Tenth Autonomous Racer
description:
img: assets/img/research/f1tenth hands-on.png
importance: 4
category: Experimental Platforms
---

The Davis Autonomous Race Car (DARC) is an innovative research platform at CORE Lab that integrates key autonomous vehicle frameworks across multiple disciplines. By combining fundamental concepts in perception, planning, control, vehicle dynamics, and real-time computing, the project has fostered a collaborative research effort between the Mechanical Aerospace Engineering and Computer Science Departments. Research teams have consistently expanded the car's capabilities, pushing the boundaries of autonomous vehicle technology through interdisciplinary innovation.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/f1tenth architecture.jpg" title="F1Tenth Racer SW Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/f1tenth hands-on.png" title="F1Tenth Hands-On" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    (Left) Software architecture of the in-house F1Tenth Davis Autonomous Race Car, DARC; (Right) Picture of the actual car we are working on
</div>

The vehicle currently drives autonomously using MPC control, and LIDAR for localization and motion planning. Current work is being done with incorporating sensor fusion using LIDAR and IMU readings with the use of an Extended Kalman Filter. By maintaining technical documentation of the software and hardware stack, the hope is that DARC will be used in live-testing more novel autonomous driving approaches. 

