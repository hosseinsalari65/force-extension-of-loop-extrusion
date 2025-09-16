# Polymer Simulation of Force-Dependent Loop-Extrusion
## Overview
This code simulates the force-dependent loop-extrusion process of Structural Maintenance of Chromosomes (SMC) complexes on a polymer chain. It models how loop extruding factors (LEFs) interact with chromatin under external force, accounting for processivity, binding, extrusion rates, and directionality.

The simulation outputs the end-to-end vector of the polymer, which can be used to study conformational changes under varying mechanical and extrusion conditions.
## Input Parameters
Each line of input.dat corresponds to one parameter, in the order below:
| Parameter  | Description                                   | Notes / Units                    |
| ---------- | --------------------------------------------- | -------------------------------- |
| **Nchain** | Chain size (number of monomers)               | Integer                          |
| **L**      | Box size                                      | Must be even                     |
| **Niter**  | Number of iterations (Monte Carlo steps)      | Integer                          |
| **Nequ**   | Number of Monte Carlo steps for equilibration | Integer                          |
| **Nmeas**  | Number of measurements                        | Integer                          |
| **Ninter** | Interval between successive measurements      | Integer                          |
| **kint**   | Bending energy                                | Energy units                     |
| **dir**    | Extrusion directionality                      | `1` = one-sided, `2` = two-sided |
| **p**      | Zero-force processivity                       |                                  |
| **ro**     | Zero-force LEF binding rate                   |                                  |
| **km0**    | Zero-force extrusion rate                     |                                  |
| **Ksmc**   | Spring constant between SMC legs              |                                  |
| **Fe**     | Characteristic force for extrusion rate       | Force units                      |
| **Fu**     | Characteristic force for unbinding rate       | Force units                      |
| **Nlef**   | Maximum number of LEFs in the system          | Integer                          |
| **Perm**   | Permeability of extruders                     | Between `0` and `1`              |
| **Fext**   | External force                                | Force units                      |
