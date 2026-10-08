---
title: "Spectral-element modeling and HPC software"
permalink: /research/computing/
toc: true
---

## Spectral-element acoustic modeling

Besides finite differences, I have implemented acoustic wave simulation with the spectral-element method, using a high-order geometric representation of the mesh.

![Spectral-element mesh with high-order geometry]({{ "/assets/images/research/sem-mesh.jpg" | relative_url }}){: .align-center}
*Mesh with high-order geometric representation.*

![P-wave velocity and density models]({{ "/assets/images/research/sem-models.jpg" | relative_url }})
*P-wave velocity model (left) and density model (right).*

![Wavefield snapshots]({{ "/assets/images/research/sem-snapshots.jpg" | relative_url }})
*Pressure wavefield snapshots at 0.04 s (left) and 0.08 s (right).*

## Performance-portable computing framework

My simulation and inversion codes share a framework that combines Kokkos with pybind11:

- **Computational core in C++ with Kokkos.** The same kernels run on CUDA, HIP, OpenMP and SYCL backends, so one code base runs on different GPUs and on CPUs.
- **Python on top through pybind11.** Top-level scripts are written in Python, which keeps experiments easy to set up while the heavy computation stays in C++.
