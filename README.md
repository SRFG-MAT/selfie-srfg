# selfie-srfg

This repository is a fork of the Selfie-Platform from the "Computational Systems Research Group" of the University of Salzburg. This project is used by Salzburg Research for external development purposes of the project RISClessNaV. For guides, tutorials and corresponding academic work please visit the original repo: https://github.com/cksystemsteaching/selfie


## Steps for working locally with both repos (selfie-srfg + selfie)

- checkout this repo and open bash in your local project repo directory
- "git remote add selfie https://github.com/cksystemsteaching/selfie.git"
- "git fetch selfie"
- "git remote -v"  -> output should look like this:
  - origin  https://github.com/SRFG-MAT/selfie-srfg.git (fetch)
  - origin  https://github.com/SRFG-MAT/selfie-srfg.git (push)
  - selfie  https://github.com/cksystemsteaching/selfie.git (fetch)
  - selfie  https://github.com/cksystemsteaching/selfie.git (push)
- "git checkout -b selfie/<name_of_selfie_branch>"

To merge Selfie-Branch changes to srfg-selfie master branch:
- pull the selfie branch that contains the desired latest changes
- checkout master branch of "selfie-srfg"
- "git merge new-branch" (fix all non-auto-merged conflicts by hand)


## Goals for this project

selfie-srfg will implement the selfie-system as a real-time environment to serve as an emergency-braking tool for an autonomously moving robot. All kernel-functions and trap handlers will be liveness-verified. The missing IO-support, OS-kernel-functionality, RT-behaviour, HW-support, trap-handling and all corresponding liveness-verification will be added in the future. Please note that this repository is still under construction and is implemented in close collaboration with Professor Christoph Kirsch (http://cs.uni-salzburg.at/~ck/) and his research team. Please note that potentially at some point within its development, this repository might differ in significant aspects from its origin.


## Used RISC-V-boards and architecture

We consider using the following hardware for this project:

- Sipeed MAix BiT (K210-architecture)

<img src="https://miro.medium.com/max/1390/1*gWbpNBY07DhTSt8nUwlnLg.jpeg" width="400" height="400" />

- HiFive Unleashed (FU540-architecture)

<img src="https://www.cnx-software.com/wp-content/uploads/2018/02/SiFive-Freedom-U540.jpg" width="400" height="400" />

- HiFive-Unmatched (FU740-architecture) - not yet supported

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQrEBagtPwyJsbhFI4b_Plbv4hwdkjQIYoPVQ&usqp=CAU" width="400" height="400" />



