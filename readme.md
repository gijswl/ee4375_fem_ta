# EE4375 - Finite Element Modelling (2022/2023)
This repository contains Jupyter notebooks with Julia and Python code for the course EE4375.
It serves as my own repository for the development of several extensions to the course material, as outlined in the official course repository (https://github.com/ziolai/finite_element_electrical_engineering).

As the development progresses, this readme and the notebooks in the repository will be extended.

## Contents
- `general`: Information about Julia in general, FEM in Julia, and gmsh
  - `gmsh`: Notebooks demonstrating how to define, generate, and visualize basic meshes with Julia and gmsh. Exercises on this subject will be added later.
    - Exercise 1: Semicircular domain for radiation problem
    - Exercise 2: Distribution transformer STEDIN
  - `julia`: Notebooks with general information about Julia and its usage for FEM.
    - The Julia programming language
    - Solving non-linear equations using ``NLsolve.jl`` and auto-differentation (e.g. ``ForwardDiff.jl``)
    - Julia for FEM with ``Gridap.jl`` and ``Ferrite.jl``
  - `misc`: Miscellaneous notebooks
    - Non-linear finite-difference method (FDM) as introduction to non-linear FEM
- `finite_difference_method`: Basic implementations of the finite difference method for electro and magnetostatics in 1D and 2D. This includes a derivation of the required differential equations and boundary conditions from Maxwell's equations, as well as discretization, solving, and post-processing of the results.
  - 1D axisymmetric electrostatics
  - 1D axisymmetric magnetostatics
  - 2D planar electrostatics
- `assignment1_fem1d`: Documentation for assignment 1 on 1-dimensional FEM with linear and quadratic elements.
  - Geometry and physics definition based on realistic inductor design
  - Derivation of stiffness & mass matrix for linear and quadratic elements
  - Global matrix assembly
  - Sparse solvers for large systems
  - Step 1: magnetostatics without eddy currents (derivation and implementation)
  - Step 2: magnetostatics with eddy currents (derivation and implementation)
  - Step 3: magnetostatics with saturation and eddy currents; model for relative permeability/BH-curve
- `assignment2_fem2d`: Documentation for assignment 2 on 2-dimensional FEM
  - Derivation of stiffness & mass matrix for linear (triangular) elements
  - Exercise 1: Distribution transformer (from [this thesis](http://resolver.tudelft.nl/uuid:15b25b42-e04b-4ff2-a187-773bc170f061))
    - Step 1: Linear magnetostatics without eddy currents
    - Step 2: Linear magnetostatics with eddy currents
    - Step 3: Non-linear magnetostatics with eddy currents
    - Step 4: Linear magnetostatics with voltage-driven coils (field-circuit coupling)
    - Step 5: Non-linear magnetostatics with voltage-driven coils (field-circuit coupling)
	- Step 6: Core and winding loss model
	- Step 7: Implementation in Gridap
	- Verification against COMSOL model from thesis
