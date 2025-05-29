---
layout: page
title: Vehicle Control
description: Modeling and control of vehicle dynamics
img: assets/img/research/at-mpc.png
importance: 1
category: Focus Areas
related_publications: true
---

## Learning MPC for Adaptive Cruise Control (ACC)
---

> {% cite abtahi2023automatic %}

Model predictive control (MPC) is a powerful tool for planning and controlling dynamical systems due to its capacity for handling constraints and taking advantage of preview information. Nevertheless, MPC performance is highly dependent on the choice of cost function tuning parameters. In this work, we demonstrate an approach for online automatic tuning of an MPC controller with an example application to an ecological cruise control system that saves fuel by using a preview of road grade. We solve the global fuel consumption minimization problem offline using dynamic programming and find the corresponding MPC cost function by solving the inverse optimization problem. A neural network fitted to these offline results is used to generate the desired MPC cost function weight during online operation. The effectiveness of the proposed approach is verified in simulation for different road geometries.

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/at-mpc.png" title="AT-MPC Results" class="img-fluid rounded z-depth-1" caption="Summary of the Automatic Tuning MPC (AT-MPC) Approach" %}
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/at-mpc-results.png" title="AT-MPC Results" class="img-fluid rounded z-depth-1" caption="Fuel economy versus average velocity for DP, AT-MPC, PT-MPC, LMPC, and PI controllers for three road profiles" %}
    </div>
</div>
<div class="caption">
    Figures from {% cite abtahi2023automatic %}
</div>

## Regnerative Braking Controller with wheel slip regulation
---

> {% cite majumdar2024sliding %}

Regenerative braking is one of the main advantages of electric propulsion systems. In such systems the vehicle brake controller has to prioritize safety while maximizing the recovered energy at all time. This paper proposes a two-step hierarchical brake controller for a dual-motor all-wheel-drive electric vehicle. In the first step a novel sliding mode controller (SMC) generates the total braking torque on each axle to independently control the slip on the front and rear wheels. In the second step the torque split controller assigns motor torques to maximize the recovered energy. The proposed SMC controller accounts for the non-linearities in vehicle dynamics and tire model, and considers the  weight transfer due to vehicle deceleration. Using simulations, we show that while the traditional SMC formulation is not effective during emergency braking scenarios, the proposed formulation successfully generates control commands to bring the vehicle to a stop position in minimum distance. Furthermore, our controller is able to maintain both wheels in the stable slip region, even when starting from a locked position. The performance of the proposed controller is evaluated for an emergency braking scenario and on an aggressive segment of the US06 cycle.

<div class="row justify-content-sm-center">
    {% include figure.liquid loading="eager" path="assets/img/research/majumdar2024sliding schematic.png" title="example image" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    Schematic of the novel SMC based regenerative wheel slip controller from {% cite majumdar2024sliding %}
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6.5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/majumdar2024sliding results1.png" title="Lock-up recovery" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5.5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/research/majumdar2024sliding results2.png" title="AT-MPC Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figures from {% cite majumdar2024sliding %} showing novel SMC performance in: (Left) recovery from wheel lock-up using the, (right) stability in low friction conditions for portion of US06 drive-cycle. 
</div>