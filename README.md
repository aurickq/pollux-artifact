# Artifact for Pollux

The artifact is contained inside `pollux-artifact.zip`. Please download this
file and extract it to view its contents:

https://github.com/aurickq/pollux-artifact/raw/c1d7d361a2f242a96d19bee433ac75f727c8aec6/pollux-artifact.zip

This artifact archive (`pollux-artifact.zip`) contains the following:

- **pollux/** contains the source code for Pollux and the scripts for setting
  up and running the testbed experiments (Section 5.2). We do not expect the
  artifact evaluator(s) to run the testbed experiments since they are costly
  and also rely on internal AWS services belonging to Petuum, Inc. Please see
  `pollux/README.md` for more details.
- **pollux-testbed.mp4** is a screen capture of a small-scale version of the
  testbed experiments running inside Petuum.
- **pollux-results/** contains raw logs collected from the testbed experiments
  described in Section 5.2. Also provided are the analysis scripts to reproduce
  Table 2, Figure 5, and Figure 6, with instructions. Please see
  `pollux-results/README.md` for more details.
- **pollux-simulator/** contains the implementation of the cluster simulator
  described in Section 5.3, instructions for reproducing the experiments shown
  in Section 5.3 and Section 5.3.2, and the analysis scripts to plot Figure 8.
  Please see `pollux-simulator/README.md` for more details.

## Getting Started Instructions

Please follow the "Getting Started" and "Checking Simulator Fidelity" sections
of `pollux-simulator/README.md`.

## Detailed Instructions

Due to the effort required to run our physical-cluster scheduling experiments,
we do not expect the artifact evaluator to do so. They also require internal
services from Petuum, Inc. which are not available publicly. The artifact
evaluator should:

- Read `pollux/README.md` to understand key files in the Pollux source code.
- Watch `pollux-testbed.mp4`, which shows a smaller-scale physical-cluster
  experiment in action.
- Review `pollux-results`, which contains raw outputs and logs from the full
  sized physical-cluster experiments. Run analysis scripts to reproduce the
  key results and figures in the paper.
- Follow the instructions in `pollux-simulator` to run and reproduce the
  simulator-based sensitivity studies presented in the paper.
