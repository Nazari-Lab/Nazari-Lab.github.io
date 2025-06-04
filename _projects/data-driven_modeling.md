---
layout: page
title: Data-Driven Modeling
description:
img: assets/img/research/gpk-concept.png
importance: 3
category: Focus Areas
related_publications: false
---

## Probabilistic Koopman Operator Modeling
---

The Koopman Operator theory is a powerful tool for obtaining approximate linear representation of complex nonlinear systems, allowing us to use the rich body of literature for linear system analysis and control on complex systems. We combine Koopman Operator theory with Gaussian Process Regression to develop non-parametric probabilistic system models that enable robust and reliable optimal control in uncertain environments. Gaussian Process observables lift the system to a higher dimensional space, where normally distributed observable functions evolve linearly under the Koopman Operator.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/gpk-concept.png" title="Conceptual Sketch of Probabilistic Koopman Model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A conceptual sketch of the probabilistic Koopman linear model compared to the deterministic Koopman linear models obtained Extended Dynamic Mode Decomposition, Direct Encoding and similar algorithms.
</div>
