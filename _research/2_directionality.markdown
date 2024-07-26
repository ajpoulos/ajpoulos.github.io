---
layout: page
title: Ground motion directionality
description: #An example project
img: /assets/img/hector_mine_v2.svg
importance: 1
category: work
---


Ground motion directionality corresponds to the variation of ground motion intensity with changes in horizontal orientation. These variations can be significant and are almost never considered in seismic risk analysis and earthquake-resistant design. For example, Figure 1 shows the variation of spectral displacement at 1 s with horizontal orientation of an example bidirectional horizontal ground motion record.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" style="max-width: 60%" src="{{ '/assets/img/Orbit.svg' | relative_url }}" alt="" title="Figure 1"/>
    </div>
</div>
<div class="caption">
    Figure 1: Relative displacement trace of a linear elastic oscillator of period 1 s subjected to an example bidirectional horizontal
ground motion record along with the variation of spectral ordinates with changes in orientation.
</div>

I first characterized these variations probabilistically using a large database of ground motion records from shallow crustal earthquakes. Figure 2 shows the variation of the response spectrum as a function of the angle from the orientation of maximum spectral response (RotD100) for the same example record of Figure 1. The intensity is normalized by the maximum intensity from all orientations (RotD100) and the median intensity (RotD50). Figure 2 also shows the variation of 99 additional records. I repeated this calculation for all records and different periods of vibration and developed statistical models for these ratios (Poulos & Miranda, 2022). These models can be used to explicitly consider ground motion directionality in future applications explicitly.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Ratios.png' | relative_url }}" alt="" title="Figure 2"/>
    </div>
</div>
<div class="caption">
    Figure 2: Pseudo-spectral acceleration at a rotation angle 𝜙 from the major response axis for an oscillator with a period of 1 s subjected to 100 recorded ground motions when normalized by (a) RotD100 and (b) RotD50.
</div>

I then studied the orientation at which the maximum horizontal intensity occurs and discovered that, for strike-slip earthquakes, this orientation tends to be close to the transverse orientation (i.e., an orientation that is perpendicular to the line segment between the recording station and the earthquake epicenter), especially at long periods (Poulos & Miranda, 2023). For example, Figure 3 presents the orientations of maximum horizontal spectral acceleration at stations that recorded the 1999 M<sub>W</sub> 7.1 Hector Mine earthquake in California, which tended to be close to the transverse orientation for most stations (i.e., most circles are blue). Very similar trends have been observed in other strike-slip earthquakes (Poulos & Miranda, 2023; Poulos & Miranda, 2024; Girmay et al., 2024; Girmay et al., 2024). These findings could affect earthquake-resistant design guidelines because current design codes do not consider a predominant horizontal orientation of ground motion. 
 
<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/hector_mine.svg' | relative_url }}" alt="" title="Figure 3"/>
    </div>
</div>
<div class="caption">
    Figure 3: Orientations of maximum horizontal spectral acceleration at 10 s (RotD100 orientations) of ground motions recorded during the 1999 M<sub>W</sub> 7.1 Hector Mine earthquake. Circles represent the location of recording stations, and their colors represent the angular distance between the RotD100 and transverse orientations. Black and gray line segments represent the RotD100 and transverse orientations, respectively.
</div>

Other directionality-related topics I worked on include the proposal of a ground motion intensity measure tailored for considering directionality in earthquake-resistant design in a simplified way (Poulos & Miranda, 2021; Poulos & Miranda, 2022), studying the role that finite duration of earthquake loading has in causing directionality (Poulos et al., 2022), and developing a model to consider directionality in ground motion models (Poulos & Miranda, 2023).

<!--- Because most ground motion models (GMMs) used nowadays use the median intensity from all horizontal orientations (known as RotD50), I then developed a statistical model that modifies RotD50 spectral accelerations given by GMMs to estimate intensities at specific horizontal orientations (Poulos & Miranda, 2023). This model depends on the angle between the orientation of interest and the transverse orientation, with the estimated intensity decreasing as the orientation of interest moves away from the transverse orientation.--->



<div class="publications">

<h3>Publications</h3>

{% bibliography -f papers -q @*[project=directionality]* --template bib_apa %}

</div>
