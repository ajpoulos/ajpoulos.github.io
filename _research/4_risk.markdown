---
layout: page
title: Seismic risk assessment
description: #An example project
img: /assets/img/Risk2.png
importance: 2
category: work
---


The goal of a probabilistic seismic risk assessment is to quantify the effect that future earthquakes will have on a system. For individual structures, this evaluation has conventionally been assessed by decoupling the problem into two parts: the evaluation of the seismic hazard at the site of the structure and the estimation of the vulnerability of the structure (i.e., its response to different ground motion intensity levels). Both results are computed independently and used together to estimate the overall risk of the structure. However, this strategy is not practical for spatially distributed infrastructure systems, such as transportation, electric power, and water distribution networks. The response of these types of systems depends on several geographically separated ground motion intensities, and the computation of their joint probability of occurrence is impractical. Thus, it is more convenient to estimate the seismic risk of these types of systems using Monte Carlo simulations, where the system is subjected to a set of earthquake scenarios. Figure 1 shows the general steps of this evaluation for an example road network. The first step is to sample a set of earthquake scenarios with corresponding ground motion intensities at the location of each component of the system. These intensities are then used to sample the damage to the components, which will reduce their functionality. Finally, the network performance is computed considering the functionality reductions. For the example system shown in the figure, the performance is characterized by the increase in travel times of the road network users.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Risk.png' | relative_url }}" alt="" title="Figure 1"/>
    </div>
</div>
<div class="caption">
    Figure 1: General seismic risk assessment steps to compute the performance of a spatially distributed system for a given earthquake scenario.
</div>

I have participated in several studies that applied this method to compute the seismic risk of several systems, including electric power networks in Chile (Espinoza et al., 2020; Ferrario et al., 2022; Oneto et al., 2024) and road networks in the San Francisco Bay Area (Silva-Lopez et al., 2022) and in Chile (Allen et al., 2022). These studies proposed some methodological advances, such as component criticality ranking (Espinoza et al., 2020), uncertainty quantification (Allen et al., 2022), and the use of neural networks to make the evaluation more efficient (Silva-Lopez et al., 2022).



<div class="publications">

<h3>Publications</h3>

{% bibliography -f papers -q @*[project=risk]* --template bib_apa %}

</div>
