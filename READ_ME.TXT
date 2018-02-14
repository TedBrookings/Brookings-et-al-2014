This directory contains the essential source code and data for the paper
Brookings T, Goeritz ML, Marder E, "Automatic parameter estimation of multicompartmental neuron models via minimization of trace error with control adjustment" J Neurophysiol. 2014 Nov 1;112(9):2332-48. doi: 10.1152/jn.00007.2014. Epub 2014 Jul 9.

All code is Copyright (c) 2014 Ted Brookings under the MIT license (see
LICENSE.TXT).

This repository is a frozen record of the code and data used for Brookings et al 2014. Any ongoing development will be done in the "fitneuron" repository at https://github.com/TedBrookings/fitneuron.

As is hopefully apparent from the accompanying paper, the code here is more proof-of-principle than practical tool. I am hoping to develop and improve this software until it is capable of reliably producing useful neuron models. No firm promises as to how long that will take, however a lot of progress has been made on speeding up/improving the integration routine, and some initial progress has been made on improving the minimization routine (which is the main source of difficulties).

All of this code has been developed on Ubuntu linux. It has been subsequently tested on RedHat linux. Although some effort has been made to avoid requiring linux, that hasn't been a major goal, and none of the code has been tested on Windows or Mac.

A non-exhaustive list of the software that is required to run this code:
- g++ 4.8.1
- OpenMpi 1.6.2
- gnu scientific library (gsl) 1.16
- matplotlib 1.2.1
- scipy 0.12.0

Supplemental contents:
- **fitneuron** Contains c++ code for fitting and simulating neuron models.
- **scripts** Contains python and matlab code for plotting and analyzing recorded/simulated traces.
- **models** Contains subdirectories for each neuron model from the paper. Each subdirectory contains necessary data and scripts to fit or simulate models, as well as a log of the outcome of the fits we performed. Keep in mind that the fits are stochastic, so exact duplication of results is not guaranteed.
- **figure 1** Contains a python script which generates the panel data for figure 1
- **figure 6** Contains a script and the basic data necessary to generate the compensation plots from figure 6
