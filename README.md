# DNAchips

DNAchips is a project to build an open source DNA synthesis chip. It is based off of an [expired patent](https://patents.google.com/patent/US6280595B1/en) from the Combimatrix Corp. They spun this technology out into a company called CustomArray, which was subsequently acquired by Genscript, and now powers their high throughput DNA synthesis pipelines. The fundamental costs of high throughput DNA synthesis - or the materials themselves - are cheap, and silicon microchips can be synthesized at an extraordinarily low cost. DNA synthesis providers have failed to make DNA synthesis more affordable over the years. We, together, can *twist* their arms into lowering prices and turnaround time by offering an alternative to the status quo that belongs to all.

## Goals

We have 4 goals with DNAchips version 1:

1. Design and synthesize a chip capable of voltage change at specific locations
2. Test a variety of conditions and buffers to create a virtual flask, visualized with bromophenol blue
3. Run a DNA synthesis process to build at least 20mers that can be used for PCR
4. Develop a protocol for testing oligo output quality (nanopore)

# Docs

## Definitions

1. Oligo: Otherwise known as "oligonucleotide" or an "oligomer". These are short pieces of DNA (or, in rare cases, RNA) that are usually synthesized chemically.
2. Virtual flask: A flask whose boundries are defined only by some arbitrary line. In our case, acid produced locally by electronics will be the flask, with boundries being buffer surrounding the electrodes, keeping the acidic conditions only in the local area around the electrode.
3. Mask: During silicon photolithography, a "mask" or "photomask" is an opaque plate with small holes that allow light to shine through. Using optics, the shadow of the plate is made extremely small. This shadow defines how a silicon chip is built.
4. Oligo pool: A pool of many individually different oligos. Usually they are synthesized on a chip using electrodes or inkjet printing, with the output getting pooled together for downstream usage.
5. Nanopore: A sequencing method that uses the electrical change of DNA as it passes through a tiny protein pore to figure out that DNA's sequence. We plan on using this sequencing method for validating our output oligos (among other methods)

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
4. [Helix: An Electrochemical CMOS DNA Synthesizer](https://ieeexplore.ieee.org/document/9830446): A modern reproduction of the technology
5. [Direct on-chip DNA synthesis using electrochemically modified gold electrodes as solid support](https://doi.org/10.7567/JJAP.57.04FM01): Deposition onto gold electrodes directly, without a porous layer
