---
layout: page
title: Research
permalink: /research/
description: 
nav: true
nav_order: 2
---

<hr class="section-separator">

My research focuses on spacecraft guidance, with broader interests spanning dynamics, control, and autonomy. I work on spacecraft rendezvous, aerocapture, interplanetary, and cislunar transfer problems. A major goal of my group is to develop fast and reliable methods for guidance, control, and onboard decision-making in future space vehicles. The challenge is to reconcile timeless mathematical ideas -- some as old as Kepler or Newton, others as new as yesterday -- with modern computational capabilities. Overall, we seek methods that can reliably guide a multimillion-dollar spacecraft far from Earth.

Feel free to reach out if you have mutual interests in any of the following:

#### <strong style='color:#BF5700'>Core research areas
- Guidance and control of aerospace vehicles
- Nonlinear dynamics and optimization
- Mechanics and dynamics of spaceflight and space science

#### <strong style='color:#BF5700'>Current projects
- Cislunar spacecraft guidance (three body, four body, and ephemeris)
- Low-thrust and impulsive trajectory optimization via sequential convex programming
- Use of solution manifolds in optimal control problems
- Pre-computing and packaging nonlinear information for onboard trajectory optimization
- Reachability and Lambert's Problem in three-body and four-body contexts

#### <strong style='color:#BF5700'>Methods
- Optimization (direct and indirect methods; convex programming)
- Automatic differentiation and differential algebra
- Perturbation theory (Straightforward, Lindstedt-Poincaré, harmonic balance)
- Coordinate transformations, parameterizations, and polynomial maps
- Linear covariance methods and other efficient uncertainty propagation techniques

<hr class="section-separator">

#### <strong style='color:#BF5700'>Gallery
Here you can browse some images and discussion from ongoing and past research projects:
<br><br>

<div class="research-gallery">
  <figure style="text-align:center; margin-bottom:2rem;">

<!-- Main image -->
<strong style="color:#BF5700; font-size:1.15rem;">Cislunar optimal trajectory design</strong><br><br>
<img src="/assets/img/drawing_2burn3burnSubmanif.png"
     alt="A continuation of 2-burn to 3-burn transfer"
     loading="lazy"
     style="width:90%; max-width:850px; height:auto; border-radius:6px;">
<!-- Figure caption text -->
<figcaption style="margin-top:1rem; text-align:left; max-width:800px; margin-left:auto; margin-right:auto;">
  <!--<strong style="color:#BF5700; font-size:1.05rem;">Cislunar optimal trajectory design</strong>-->
  This work leverages the existence of various types of "solution submanifolds", which parameterize smooth variations of the solutions to optimal control problems. In the example application depicted above, we compute a delta-V optimal three-burn transfer between two halo orbits. For these types of problems, the optimal number and timing of the interior maneuvers is not obvious a priori. However, this can be solved quickly and easily. First, an initial 2-burn transfer is computed via a reachability-based approach, and then we make use of a smooth 1D path between the 2-burn and 3-burn solutions. The intermediate solutions are solved via a "monomial method" first introduced at the AAS Astrodynamics Specialist Conference in 2024. This can be extended to accommodate any number of maneuvers which the optimum may possess.
  <br>
  <span style="color:#BF5700; font-weight:500;">
  ↳ Work in preparation (2026)
  </span>
</figcaption>
  </figure>
</div>
<hr style="border: none; border-top: 1px solid #ddd; margin: 2.5rem auto; width: 90%;">

<div class="research-gallery">
<figure style="text-align:center;">
<strong style="color:#BF5700; font-size:1.15rem;">Modal decomposition of spacecraft relative motion</strong><br><br>
<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/drawing_ModalDecomp.png"
       alt="Modal decomposition of spacecraft relative motion — top panel"
       loading="lazy"
       style="width:55%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    Modal decomposition of satellite relative motion is analogous to that of a vibrating beam.
  </div>
</div>

<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/drawing_JGCD_cisl.png" 
       alt="Application to relative motion control — bottom panel"
       loading="lazy"
       style="width:90%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    Application to relative motion control near an L2 halo orbit.
  </div>
</div>

<figcaption style="margin-top:0.8rem; text-align:left; max-width:800px; margin-left:auto; margin-right:auto;">
  As part of my PhD thesis, I developed a <em>modal theory</em> of close-proximity spacecraft relative motion. By this perspective, the relative motion of one spacecraft in the vicinity of another can be decomposed into a finite number of physically realizable "mode shapes". These are useful for control design and analysis. This methodology can be applied to the linearized dynamics about any closed (periodic) orbit. This work leveraged Lyapunov–Floquet theory, which is used to identify a mapping from a time-periodic linear system to a time-invariant counterpart. Impulsive guidance solutions are rapidly obtained as the solution to a second-order cone program (SOCP).
  <br>
  <a href="https://doi.org/10.2514/1.G006603" target="_blank"
     style="color:#BF5700; font-weight:500; text-decoration:none;">
    ↳ Journal paper (J. Guidance, Control, and Dynamics, 2022)
  </a>
  &nbsp;|&nbsp;
  <a href="https://www.hanspeterschaub.info/PapersPrivate/Burnett2022d.pdf" target="_blank"
     style="color:#BF5700; font-weight:500; text-decoration:none;">
    Repository preprint
  </a>
    </figcaption>
  </figure>
</div>
<hr style="border: none; border-top: 1px solid #ddd; margin: 2.5rem auto; width: 90%;">

<div class="research-gallery">
<figure style="text-align:center;">
	<strong style="color:#BF5700; font-size:1.15rem;">Chance-constrained, drift-safe guidance for spacecraft rendezvous</strong><br><br>
<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/drawing_BlueTraj1.png"
       alt="Some rendezvous trajectories — top panel"
       loading="lazy"
       style="width:90%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    Chance-constrained drift-safe spacecraft rendezvous trajectories.
  </div>
</div>

<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/drawing_BlueTraj2.png"
       alt="LinCov — bottom panel"
       loading="lazy"
       style="width:60%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    3-sigma uncertainty bounds, propagated via LinCov method.
  </div>
</div>

<figcaption style="margin-top:0.8rem; text-align:left; max-width:800px; margin-left:auto; margin-right:auto;">
  This work, conducted with colleagues at Blue Origin, explored both fuel and time-optimal close-proximity rendezvous guidance solutions that are <em>drift safe</em> -- meaning that in the event of a missed maneuver, the trajectory will safely miss the target-centered keep-out sphere (KOS). This is depicted in the top figures where nominal trajectories are given by black lines, 3-sigma dispersions are in green, and the KOS is a red circle. This work accounted for expected starting state dispersions, navigation error, and maneuver execution error. Uncertainties were propagated efficiently using a Linear Covariance ("LinCov") approach. This is depicted in the bottom figure. The trajectories were solved using sequential convex programming (SCP), which easily accommodates various constraints.
  <br>
  <a href="https://doi.org/10.48550/arXiv.2401.11077" target="_blank"
     style="color:#BF5700; font-weight:500; text-decoration:none;">
    ↳ Paper (AAS Rocky Mountain GN&C Conference, 2022)
  </a>
    </figcaption>
  </figure>
</div>
<hr style="border: none; border-top: 1px solid #ddd; margin: 2.5rem auto; width: 90%;">

<div class="research-gallery">
<figure style="text-align:center;">
<strong style="color:#BF5700; font-size:1.15rem;">Aerocapture computational guidance</strong><br><br>
<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/aerocapture_earth_test.png"
       alt="Aerocapture Earth test — top panel"
       loading="lazy"
       style="width:65%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    Artistic depiction of aerocapture technology Earth-based test. 
  </div>
</div>

<div style="margin-bottom:0.7rem;">
  <img src="/assets/img/drawing_AerocaptureGuidance.png"
       alt="Guidance algorithm flowcharts — bottom panel"
       loading="lazy"
       style="width:85%; max-width:800px; height:auto; border-radius:6px;">
  <div style="font-size:0.9rem; color:#444; margin-top:0.3rem;">
    Comparison of traditional predictor-corrector guidance (left) vs. experimental guidance approach (right).
  </div>
</div>

<figcaption style="margin-top:0.8rem; text-align:left; max-width:800px; margin-left:auto; margin-right:auto;">
  This work, conducted with colleagues at NASA JPL, introduced a computationally efficient guidance method for aerocapture drag skirt jettison timing. In typical interplanetary trajectory design, a spacecraft will conduct an orbital insertion maneuver to slow down and enter orbit upon arrival at a target planet. In <em>aerocapture</em>, a spacecraft is instead packed into an aeroshell, and is carefully flown through the upper atmosphere of the target planet to reduce its interplanetary speed. The exact amount of slow-down, and hence the resulting planetary orbit, should be controlled by carefully timing of the jettison of a drag skirt (depicted in top figure). In such an environment, the ideal jettison time must be calculated onboard, during atmospheric flight, via a guidance algorithm run at high frequency for maximum timing accuracy. In this work, we introduced a novel algorithm whose computational footprint can be easily profiled, and is expected to be lighter than a predictor-corrector approach, but without sacrificing guidance accuracy. The completely deterministic algorithm is in the right panel above, with the legacy predictor-corrector approach in the left panel.
  <br>
  <a href="https://doi.org/10.1016/j.asr.2023.09.034" target="_blank"
     style="color:#BF5700; font-weight:500; text-decoration:none;">
    ↳ Journal paper (Advances in Space Research, 2023)
  </a>
  &nbsp;|&nbsp;
  <a href="https://hanspeterschaub.info/PapersPrivate/Albert2023c.pdf" target="_blank"
     style="color:#BF5700; font-weight:500; text-decoration:none;">
    Repository preprint
  </a>
    </figcaption>
  </figure>
</div>
<hr style="border: none; border-top: 1px solid #ddd; margin: 2.5rem auto; width: 90%;">
