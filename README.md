# selfie-srfg

This repository is a fork of the Selfie-Platform from the "Computational Systems Research Group" of the University of Salzburg. The "master"-branch of the project is used by Salzburg Research for external development purposes of the project RISClessNaV. The "origin"-branch points to the "master"-branch of the original selfie-repo. Changes made to the original selfie repository by the "Computational Systems Research Group" can be integrated likewise, if needed. 

For guides, tutorials and corresponding academic work please visit the original repo: https://github.com/cksystemsteaching/selfie


## Goals for this project

selfie-srfg will implement the selfie-system as a real-time environment to serve as an emergency-braking tool for an autonomously moving robot. All kernel-functions and trap handlers will be liveness-verified. The missing IO-support, OS-kernel-functionality, RT-behaviour, HW-support, trap-handling and all corresponding liveness-verification will be added in the future. Please note that this repository is still under construction and is implemented in close collaboration with Professor Christoph Kirsch (http://cs.uni-salzburg.at/~ck/) and his research team. Please note that potentially at some point within its development, this repository might differ in significant aspects from its origin.


## Used RISC-V-boards and architecture

We consider using the following hardware for this project:
- Sipeed MAix BiT (K210-architecture)
- HiFive Unleashed (FU540-architecture)
- HiFive-Unmatched (FU740-architecture) - not yet supported
