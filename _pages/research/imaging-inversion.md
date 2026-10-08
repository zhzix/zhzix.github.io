---
title: "Imaging and inversion"
permalink: /research/imaging-inversion/
toc: true
---

Institute of Acoustics, Chinese Academy of Sciences · with Dr. Peng Yong

## Joint full-waveform inversion

Since September 2025. My thesis topic is full-waveform inversion based on scale separation. Joint full-waveform inversion (JFWI) splits the model into a smooth background and a perturbation, and uses both transmitted and reflected waves to update them. I work on robust misfit functions for this framework.

I have an initial JFWI implementation, tested on an anomaly model and on the Marmousi model.

![Sensitivity kernels under two parameterizations]({{ "/assets/images/research/jfwi-kernels.jpg" | relative_url }})
*Sensitivity kernels under the velocity (left) and impedance (right) parameterizations.*

![JFWI test on an anomaly model]({{ "/assets/images/research/jfwi-anomaly.jpg" | relative_url }})
*Anomaly model. Left to right: true model, inverted velocity, inverted impedance perturbation.*

![JFWI test on the Marmousi model]({{ "/assets/images/research/jfwi-marmousi.jpg" | relative_url }})
*Marmousi model: inverted velocity (left) and inverted impedance perturbation (right).*

## Misfit functions and optimization

I have run preliminary inversion tests with optimal-transport (OT) and localized adaptive waveform inversion (LAWI) misfit functions, including a preliminary 3-D test on field data. I have also tested local optimization methods (steepest descent, conjugate gradient, L-BFGS, with line search and trust region) and global ones (simulated annealing, genetic algorithm, particle swarm).

## Ultrasonic imaging of rock samples

Since October 2025.

- 3-D ultrasonic phased-array imaging of rock blocks from full-matrix capture data (16-element transmit/receive arrays), using IQ demodulation and delay-and-sum beamforming, with Kirchhoff migration as a comparison.
- Processing of laboratory datasets, including ultrasonic monitoring of CO<sub>2</sub>–water displacement in rock cores.
