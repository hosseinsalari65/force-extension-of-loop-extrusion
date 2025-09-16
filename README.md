# Polymer Simulation of Force-Dependent Loop-Extrusion
## Overview
This code simulates the force-dependent loop-extrusion process of Structural Maintenance of Chromosomes (SMC) complexes on a polymer chain. It models how loop extruding factors (LEFs) interact with chromatin under external force, accounting for processivity, binding, extrusion rates, and directionality.

The simulation outputs the end-to-end vector of the polymer, which can be used to study conformational changes under varying mechanical and extrusion conditions.
## Input Parameters
Each line of input.dat corresponds to one parameter, in the order below:
| Parameter  | Description                                                | 
| ---------- | -----------------------------------------------------------| 
| **Nchain** | Chain size (number of monomers) (in kbp)                   | 
| **L**      | Box size (in 28.2 nm)                                      | 
| **Niter**  | Number of iterations (Monte Carlo steps)                   |
| **Nequ**   | Number of Monte Carlo steps for equilibration              |
| **Nmeas**  | Number of measurements                                     |
| **Ninter** | Interval between successive measurements                   | 
| **kint**   | Bending energy (in k_BT)                                   | 
| **dir**    | Extrusion directionality (`1` = one-sided, `2` = two-sided)| 
| **p**      | Zero-force processivity (in kbp)                           |
| **ro**     | Zero-force LEF binding rate (between `0` and `1`)          |
| **km0**    | Zero-force extrusion rate (in 1000 kbp/s)                  |
| **Ksmc**   | Spring constant between SMC legs (in 0.062 pN/nm)          |
| **Fe**     | Characteristic force for extrusion rate (in 0.13 pN)       | 
| **Fu**     | Characteristic force for unbinding rate (in 0.13 pN)       | 
| **Nlef**   | Maximum number of LEFs in the system                       |
| **Perm**   | Permeability of extruders (Between `0` and `1`)            | 
| **Fext**   | External force (in 0.13 pN)                                | 
