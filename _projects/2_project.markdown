---
layout: page
title: Flow estimation
description: Estimating a fluid flow from solute observations
img: /assets/img/juq_histmatrix_3x3.png
importance: 2
---

The goal of this project was to estimate a fluid flow from (noisy, finite)
observations of a solute (e.g., a pollutant or dye) advecting and diffusing in
the fluid. Here the goal was to estimate incompressible flow $$\mathbf{v}$$
from observations of solute concentration $$\theta$$ governed by the
two-dimensional advection-diffusion equation: 
$$
\frac{\partial}{\partial t} \theta = -\mathbf{v} \cdot \nabla \theta + \kappa \Delta \theta
$$

This problem was sort of a playground to test out the framework for
Bayesian inversion for infinite-dimensional unknowns, as well as Markov Chain
Monte Carlo methods designed for those applications, from
perspectives ranging from the highly computational (GPU-based algorithms) to 
the highly theoretical (long proof-based paper).  

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/juq_bigrun_003_0067.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/jcp_particle2d_00098.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/juq_histmatrix_3x3.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
   Left: An example solution concentration. Middle: Simulated solute particle movement. Right: A selection of correlation plots from an example posterior measure.
</div>
