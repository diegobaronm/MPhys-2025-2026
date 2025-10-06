# MPhys-2025-2026
This stores relevant info/instructions/docs/code for the MPhys project 2025/26 at The University of Manchester

<img width="388" height="259" alt="image" src="https://cds.cern.ch/record/2299951/files/feynman_ttbar_emu.png" />

## Members
Students: Jaicob Fairham, Peter Zeman

Supervisors: Diego Baron, Valentina Vecchio, Yvonne Peters

## Goal
We will explore how ML techniques can benefit the calibration of jet-flavour tagging algorithms in the ATLAS collaboration (GN2v01). Some of the objectives include:
- Understanding the outputs of the ttbar di-lepton (ttbar2L) ATLAS simulation for Run2 and Run3.
- Select a sample of fully-matched ttbar2L events.
- Apply the HyPER algorithm to this sample and measure/compare its performance.
- Explore modifications/different ML approaches to enhance the reconstruction and signal/background discrimination.
- Construct and perform a fit to measure the efficiency of GN2 in real ATLAS data and compare it to the MC samples to derive a calibration.

## Relevant literature
- [ATLAS b-calibration](https://arxiv.org/abs/1907.05120)
- [GN2](https://arxiv.org/abs/2505.19689)
- [HyPER](https://arxiv.org/abs/2402.10149)


## Material (code/docs)

- [FastFrames](https://atlas-project-topreconstruction.web.cern.ch/fastframesdocumentation/latest/): A tool for converting ROOT ntuples into 1D/2D histograms or more ntuples! See two tutorials [here](https://atlas-project-topreconstruction.web.cern.ch/fastframesdocumentation/latest/tutorial/) and [here](https://atlas-project-topreconstruction.web.cern.ch/fastframesdocumentation/latest/eventtutorials/topws2025/Tutorial/).
- [HyPER](https://github.com/tzuhanchang/HyPER/tree/main): The reconstruction algorithm we want to try.
- Quick install FastFrames, [here](https://gitlab.cern.ch/dbaronmo/fastfastframessetup).
- [This code](https://gitlab.cern.ch/dbaronmo/atlastohyper) holds the workflow we used to train the ttbar all-hadronic and single-lepton final states.
