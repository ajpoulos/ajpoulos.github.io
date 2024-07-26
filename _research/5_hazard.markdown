---
layout: page
title: Seismic source modeling
description: #An example project
img: /assets/img/Recurrence_model.png
importance: 2
category: work
---


Seismic source models are a critical input for any probabilistic seismic hazard analysis, which in turn enables the estimation of seismic risk. These models contain the geometry of the seismic sources and their magnitude-frequency distributions or earthquake recurrence relationships. I developed one of these models for subduction earthquakes in Chile using an earthquake catalog with seismic events up to 2018 (Poulos et al., 2019). I divided the seismicity into seven zones shown in Figure 1: three for subduction interface earthquakes, which occur in the interface between the subducting Nazca Plate and the continental South American Plate; and four for subduction intraslab earthquakes, which occur within the subducting Nazca Plate at intermediate depths. Figure 1 also shows the magnitude-frequency distributions for each zone, which, in this case, correspond to Gutenberg-Richter relations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Recurrence_model.png' | relative_url }}" alt="" title="Figure 1"/>
    </div>
</div>
<div class="caption">
    Figure 1: Seismic sources used to represent subduction seismicity in Chile and their calibrated Gutenberg-Richter relations.
</div>

To compare the developed model with previous models, I combined all interface and intraslab sources, resulting in the two Gutenberg-Richter relations shown in Figure 2. The seismicity rates of the developed model are similar to some previous models (i.e., Martin, 1990; Núñez, 2014). However, surprisingly, the rates reported by Barrientos (1980) are one order of magnitude lower, and those reported by Leyton et al. (2009) are one order of magnitude higher. Thus, these models must be used with caution.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Compare_rates.svg' | relative_url }}" alt="" title="Figure 2"/>
    </div>
</div>
<div class="caption">
    Figure 2: Comparison of recurrence relations for Chilean (a) interface and (b) intraslab seismicity relative to previous models. The relations from Barrientos (1980), Martin (1990), and Leyton et al. (2009) had to be transformed from surface-wave magnitude to moment magnitude.
</div>


<div class="publications">

<h3>Publications</h3>

{% bibliography -f papers -q @*[project=hazard]* --template bib_apa %}

</div>
