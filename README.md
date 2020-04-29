# Extreme regime detection
The aim of this project is the automatic load adding in the node and search of extreme regimes, i.e. loss of static stability.

## Installation
 - install MATPOWER 7.0 https://matpower.org/download/
 - include the adopted versions of runpf.m and newtonpf.m in the current path

## Changes to MATPOWER library files
 Based on the MATPOWER 7.0 the files runpf.m and newtonpf.m are adopted.
 

## Test simulations using IEEE14
To run the simulation for the [IEEE14](https://electricgrids.engr.tamu.edu/electric-grid-test-cases/ieee-14-bus-system/) test grid run 
```
 IEEE14.m
```
from the MATLAB prompt. Here, the user can select a number of parameters:
 - load node to investigate (default indicated in the command window after running the program),
 - accuracy of calculation (default [0.001;1]),
 - power increment (default [1;100] MW).

After a successful calculation the graphs of the Jacobian determinant |J| and its second derivative |J''| are shown. 

Also in the command window a power range is displayed, where the limit mode for static aperiodic stability is located.
