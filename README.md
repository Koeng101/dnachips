# DNAchips

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![UPRJ_CI](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml) [![Caravel Build](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml)

DNAchips is a project to build an open source DNA synthesis chip. It is based off of an [expired patent](https://patents.google.com/patent/US6280595B1/en) from the Combimatrix Corp. They spun this technology out into a company called CustomArray, which was subsequently acquired by Genscript, and now powers their high throughput DNA synthesis pipelines. The fundamental costs of high throughput DNA synthesis - or the materials themselves - are cheap, and silicon microchips can be synthesized at an extraordinarily low cost. DNA synthesis providers have failed to make DNA synthesis more affordable over the years. We, together, can *twist* their arms into lowering prices and turnaround time by offering an alternative to the status quo that belongs to all.

## Goals

We have 4 goals with DNAchips version 1:

1. Design and synthesize a chip capable voltage change at specific locations
2. Test a variety of conditions and buffers to create a "virtual flask", visualized with bromophenol blue
3. Run a DNA synthesis process to build at least 20mers that can be used for PCR
4. Develop a protocol for testing oligo output quality (nanopore)

# Docs

## Words

1. Virtual flask: 

## Tooling
1. [chisel3](https://github.com/chipsalliance/chisel3) Higher level Verilog design
2. [caravel example project](https://github.com/efabless/caravel_user_project) An example project using caravel, the base for efabless chipignite
3. [google-skywater pdk](https://github.com/google/skywater-pdk) The google skywater PDK, used by chipignite

## Resources

### Fab
1. [efabless overview](https://youtu.be/FlwX4kVewkA) A high level overview of efabless as a company
2. [chipignite](https://efabless.com) Chipignite, the service we would use to synthesize our chips
3. [si130nm](https://j.mp/si130nm) Inspirational doc on the 130nm process
4. [walkthrough of efabless](https://www.youtube.com/watch?v=MNuoYz_MM-c) A walkthrough using a user project with efabless

### DNA
1. [Webinar: Oligo pools design, synthesis, and research applications](https://www.youtube.com/watch?v=gAH2kwvc7vM): A webinar on the electrochemical synthesis technology
2. [DNA synthesis on electrochemical chips](https://doi.org/10.1371/journal.pone.0000034): The original DNA synthesis on electrochemical chip paper
3. [DNA synthesis using electrodes patent](https://patents.google.com/patent/US6280595B1/en): The original DNA synthesis patent (expired)

# Caravel docs

Refer to [README](docs/source/quickstart.rst) for a quick start of how to use caravel_user_project
Refer to [README](docs/source/index.rst) for this sample project documentation. 
