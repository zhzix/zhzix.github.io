---
title: "Seismic wave modeling with topography"
permalink: /research/overset-seismic/
toc: true
---

Since September 2023 · School of Geosciences, China University of Petroleum (East China) · with Prof. Jianping Huang and Dr. Peng Yong

## Overview

Surface topography is hard to handle with a single Cartesian finite-difference grid. I developed an overset Virieux–Lebedev grid finite-difference time-domain (FDTD) scheme for elastic wave simulation: a surface-following grid represents the topography and overlaps a background Cartesian grid that covers the rest of the model. The scheme was first developed in 2-D and then extended to 3-D.

## 2-D: SEG Foothills model

The 2-D scheme is tested on the SEG Foothills model and compared with a spectral-element reference computed with SPECFEM2D and with a single-grid simulation.

![SEG Foothills model]({{ "/assets/images/research/foothills-model.jpg" | relative_url }})
*The SEG Foothills model used for the 2-D test.*

![Seismogram comparison on the SEG Foothills model]({{ "/assets/images/research/foothills-seismograms.jpg" | relative_url }})
*Seismograms at six receivers: SPECFEM2D reference, single grid and overset grid.*

![Wavefield snapshots on the SEG Foothills model]({{ "/assets/images/research/foothills-snapshots.jpg" | relative_url }})
*Wavefield snapshot comparison.*

## 3-D: crustal model with topography

The 3-D extension is tested on a 3-D crustal model with surface topography, comparing the overset grid with a single-grid simulation.

![3-D crustal model]({{ "/assets/images/research/crustal3d-model.jpg" | relative_url }})
*The 3-D crustal model.*

![Seismogram comparison on the 3-D crustal model]({{ "/assets/images/research/crustal3d-seismograms.jpg" | relative_url }})
*Three-component seismograms: single grid and overset grid.*

![Wavefield snapshots on the 3-D crustal model]({{ "/assets/images/research/crustal3d-snapshots.jpg" | relative_url }})
*Wavefield snapshot comparison.*

## Publications

- **Zixiao Zhang**, Peng Yong, Jianping Huang. Efficient 3-D Seismic Wave Simulation in the Presence of Topography Using an Overset Virieux–Lebedev Grid FDTD Scheme. *Geophysical Journal International*, 2026, 246(3), ggag274.
- **Zixiao Zhang**, Peng Yong, Jianping Huang. An Overset Virieux–Lebedev Finite-Difference Time-Domain Scheme for Efficient Seismic Wave Modeling in Complex Topography. *Geophysics*, 2026, 91(5), T207–T224.
