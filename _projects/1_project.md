---
layout: page
title: Vehicle Control
description: Modeling and control of vehicle dynamics
img: assets/img/research/at-mpc.png
importance: 1
related_publications: true
---

# Learning MPC for Adaptive Cruise Control (ACC) {% cite abtahi2023automatic %}
Model predictive control (MPC) is a powerful tool for planning and controlling dynamical systems due to its capacity for handling constraints and taking advantage of preview information. Nevertheless, MPC performance is highly dependent on the choice of cost function tuning parameters. In this work, we demonstrate an approach for online automatic tuning of an MPC controller with an example application to an ecological cruise control system that saves fuel by using a preview of road grade. We solve the global fuel consumption minimization problem offline using dynamic programming and find the corresponding MPC cost function by solving the inverse optimization problem. A neural network fitted to these offline results is used to generate the desired MPC cost function weight during online operation. The effectiveness of the proposed approach is verified in simulation for different road geometries.

<div class="d-flex justify-content-center">
    {% include figure.liquid
        path="assets/img/research/at-mpc.png"
        title="AT-MPC Concept"
        width="600px"
        caption="Summary of the Automatic Tuning MPC (AT-MPC) approach"
        class="rounded z-depth-1"
    %}
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/at-mpc-results.png" title="AT-MPC Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Fuel economy versus average velocity for DP, AT-MPC, PT-MPC, LMPC, and PI controllers for three road profiles {% cite abtahi2023automatic %}
</div>

