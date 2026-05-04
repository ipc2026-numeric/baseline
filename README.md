# ENHSP Baselines for IPC


This folder contains an example of how to structure a planner submission to the numeric track of the IPC 2026.

It contains the following:
- A src directory (empty in this example)
- An apptainer Recipe
- Different run scritps indicating the specific sub-track (sat(isficing), opt(timal), agile) and the supported fragment of numeric planning (SNP or LNP).


## Installation

Assuming that you have the source files for enhsp located in `/src/enhsp`, run the following command:

```sudo apptainer build enhsp.sif Recipe```

This will create qn executable file, ```enhsp.sif```, which will be the main entry point for the ```run``` scripts (included in this repositiory).

Note that the recipe also specifies how the planner should be executed (see the ```%runscript``` section).