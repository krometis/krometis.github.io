---
layout: page
title: Statistical shape estimation
description: Statistical estimation of boundary shapes from fluid, solute, or acoustic information
img: /assets/img/svsector_013_radii_quantiles.png
importance: 3
---

The goal of this line of research has been to estimate the shape of a domain from (noisy, finite) data describing:
- A fluid in the domain
- A solute (e.g., a pollutant or dye) advecting and diffusing in the fluid
- Acoustics (e.g., resonant frequencies) of the domain

While traditional methods of shape estimation have been well-established, we apply the Bayesian approach to parameter estimation. In doing so, we can incorporate prior knowledge from, e.g., theoretical properties or previous measurements, in addition to the data to characterize the shape of the associated domain. In contrast to traditional methods, the Bayesian approach also provides estimates of uncertainty, which can provide critical context to the results, such as whether there are unresolved degrees of freedom, such as when a class of shapes matches the data and prior information. These additional degrees of freedom can help dictate further data collection that might refine the unknown shape or, when applied to design problems, additional considerations (e.g., aesthetics) that might be accommodated while still matching the data.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/vortsensor_017_sample_grid_vort.png' | relative_url }}" alt="" title="vorticity matching"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/svsector_013_radii_quantiles.png' | relative_url }}" alt="" title="scalar matching"/>
    </div>
</div>
<div class="caption">
   Left: Rotor shapes that produce similar vorticities at a set of sensor locations. Right: Posterior radius quantiles for matching solute scalar variance by sector.
</div>

<strong>Relevant Publications:</strong>
<ul>
<li>Borggaard, Jeff, Nathan E. Glatt-Holtz, and Justin Krometis. “A Statistical Framework for Domain Shape Estimation in Stokes Flows.” Inverse Problems 39, no. 8 (June 2023): 085009. <a href="https://doi.org/10.1088/1361-6420/acdd8e">https://doi.org/10.1088/1361-6420/acdd8e</a>.</li>
</ul>
