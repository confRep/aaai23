# Verification of relational action bases

This repository contains a benchmark set for safety checking of relational action bases (RABs for short). 
Each file in the set consists of a RAB model specification and a corresponding (un)safety property to verify. 
The provided files can be immediately tested using the latest version of the [MCMT model checker](http://users.mat.unimi.it/users/ghilardi/mcmt/).

## How to run MCMT?
MCMT is an SMT-based model checker that supports verification of infinite-state transition systems. One can download it [here](http://users.mat.unimi.it/users/ghilardi/mcmt/license.html).
 Consult MCMT's [user manual](http://users.mat.unimi.it/users/ghilardi/mcmt/UM_MCMT_3.0.pdf) for more information on the tool itself.
 MCMT has to be linked to the SMT solver [Yices 1](https://yices.csl.sri.com/) which has to be downloaded separately. 
 To run a file with a RAB model and test its safety, use the command line and type this: `./bin/mcmt [options] <filename>`.
