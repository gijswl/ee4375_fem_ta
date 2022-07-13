# EE4375 - Finite Element Modelling (2022/2023)
This repository contains Jupyter notebooks with Julia and Python code for the course EE4375.
It serves as my own repository for the development of several extensions to the course material, as outlined in the official course repository (https://github.com/ziolai/finite_element_electrical_engineering).

As the development progresses, this readme and the notebooks in the repository will be extended.

## Contents
- general: Information about Julia in general, FEM in Julia, and gmsh
  - gmsh: Notebooks demonstrating how to define, generate, and visualize basic meshes with Julia and gmsh. Exercises on this subject will be added later.
  - julia: Notebooks with general information about Julia and its usage for FEM.
    - Solving non-linear equations using ``NLsolve.jl`` and auto-differentation (e.g. ``ForwardDiff.jl``)
    - Julia for FEM with ``Gridap.jl`` and ``Ferrite.jl``
  - misc: Miscellaneous notebooks
    - Non-linear finite-difference method (FDM) as introduction to non-linear FEM
- assignment1_fem1d: Documentation for assignment 1 on 1-dimensional FEM with linear and quadratic elements.
  - Geometry and physics definition based on realistic inductor design
  - Derivation of stiffness & mass matrix for linear and quadratic elements
  - Step 1: magnetostatics without eddy currents (derivation and implementation)
  - Step 2: magnetostatics with eddy currents (derivation and implementation)
  - Step 3: magnetostatics with saturation and eddy currents; model for relative permeability/BH-curve
