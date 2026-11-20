<img width="900" height="650" alt="fine_Ma_8e-05" src="https://github.com/user-attachments/assets/c76df65e-e244-4fc9-a892-968cdd5e53bb" />
<img width="900" height="650" alt="fine_T_8e-05" src="https://github.com/user-attachments/assets/26392c4b-30b8-4d1e-9df2-d3c12a0ac639" />
<img width="900" height="650" alt="fine_rho_8e-05" src="https://github.com/user-attachments/assets/100f447f-42cf-4122-9184-c617776aad1c" />
# rhoCentralFoamODW
Modified rhoCentralFoam with a simplified two-step Xi chemistry model for double-wedge oblique detonation simulations.
# rhoCentralFoamODW

A modified OpenFOAM solver for numerical investigation of
oblique detonation wave (ODW) formation in a double-wedge geometry.

## Overview

`rhoCentralFoamODW` is a modified version of OpenFOAM's
`rhoCentralFoam`, developed to investigate compressible reacting
flow and oblique detonation phenomena in a double-wedge configuration.

The solver incorporates a simplified two-step chemistry model using
an additional progress variable, `Xi`, to represent the evolution of
the reactive mixture.

This implementation is intended for numerical investigation of
ODW-related flow physics and is not a detailed H2-air chemical
kinetics solver.

## Main Features

- Modified `rhoCentralFoam` framework
- Compressible reacting-flow formulation
- Additional reaction-progress variable `Xi`
- Simplified two-step reaction mechanism
- Double-wedge ODW configuration
- OpenFOAM-based numerical simulation and post-processing

## Chemistry Model

The present implementation uses a reduced two-step chemistry model
rather than a detailed H2-air reaction mechanism.

The variable `Xi` is introduced as a reaction-progress variable to
represent the evolution of the chemical state through the simplified
reaction scheme.

The model is intended to capture the essential coupling between
compressible flow, heat release, and detonation-wave dynamics while
avoiding the computational cost of detailed chemical kinetics.

## Case Description

The repository includes a double-wedge configuration used to study
oblique detonation wave development.

The simulation case includes the required OpenFOAM initial conditions,
physical properties, chemistry parameters, mesh generation and solver
settings.

## Repository Structure

- `src/` — modified `rhoCentralFoamODW` solver source code
- `tutorials/doubleWedgeODW/` — double-wedge simulation case
- `chemistry/` — documentation and parameters for the simplified
  chemistry model
- `postProcessing/` — selected analysis and visualization materials

## Important Note

This repository does not implement a detailed H2-air chemical kinetic
mechanism. The chemistry is intentionally simplified using a
two-step reaction model with the `Xi` progress variable.

## Status

Research code developed for numerical investigation of
oblique detonation wave phenomena.
