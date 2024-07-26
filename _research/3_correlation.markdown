---
layout: page
title: Correlations of spectral accelerations
description: #An example project
img: /assets/img/Surfaces_2.png
importance: 3
category: work
---


Ground motion models provide a marginal probability distribution of a ground motion intensity measure (e.g., a spectral acceleration at a specific period), given rupture and site parameters (e.g., earthquake magnitude and source-to-site distance). However, several applications require the joint probability distribution of these intensity measures, such as vector-valued probabilistic seismic hazard analysis and constructing conditional spectra. Assuming that the logarithm of these intensity measures has a multivariate normal distribution, their joint probability distribution can be constructed by knowing the correlations between them. We estimated these correlations for spectral accelerations of different periods using ground motion records from subduction earthquakes in Chile (Candia et al., 2020). These correlations depend on the two periods of the corresponding spectral accelerations. We also developed the first model for these correlations that depends on the damping ratio (Poulos & Miranda, 2023). Previous models only considered 5% damping. Our model now depends on four variables, that is, the two periods and the two damping ratios of the corresponding spectral accelerations. Figure 1 shows the sensitivity of the correlations to both damping ratios for four different combinations of periods.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Surfaces.png' | relative_url }}" alt="" title="Figure 1"/>
    </div>
</div>
<div class="caption">
    Figure 1: Correlations between spectral accelerations at T<sub>1</sub> = 1 s and spectral accelerations at: (a) T<sub>2</sub> = 0.1 s, (b) T<sub>2</sub> = 0.3 s, (c) T<sub>2</sub> = 1 s, and (d) T<sub>2</sub> = 3 s, as a function of the damping ratios in the two oscillators.
</div>


<div class="publications">

<h3>Publications</h3>

{% bibliography -f papers -q @*[project=correlation]* --template bib_apa %}

</div>
