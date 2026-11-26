---
title: "Spectral-element modeling and HPC software"
permalink: /research/computing/
toc: true
---

## Spectral-element wave modeling

Besides finite differences, I have implemented wave simulation with the spectral-element method, using a high-order geometric representation of the mesh. The solver covers acoustic, elastic and TTI pseudo-acoustic wave equations.

## Performance-portable computing framework

My simulation and inversion codes share a framework that combines Kokkos with pybind11:

- **Computational core in C++ with Kokkos.** The same kernels run on CUDA, HIP, OpenMP and SYCL backends, so one code base runs on different GPUs and on CPUs.
- **Python on top through pybind11.** Top-level scripts are written in Python, which keeps experiments easy to set up while the heavy computation stays in C++.
