# Week 5

Outcomes from previous week:
- The students presented slides, showing plots produced with FastFrames using the `.yaml` configuration.
- The students understand the contents of the datasets better and how to handle the data collections.

Discussion:
- The students presented slides.
- We clarified that the meeting slot should be exclusively reserved unless very urgent matters need attention.
- Diego gave a brief explanation of how to move the `yaml` code to the C++ custom class.

Plan for next week:
- The students will implement all the selection cuts described in the calibration paper using the C++ custom class framework. Using the Mini-Analysis feature of FastFrames is useful to track the selections.
- Peter will implement the chi-squared routine to define the reconstruction performance baseline. He will also check that the truth deltaR matching provided by the code is correct.
- Jacob will use the matching provided in the datasets to define the truth labels for the reconstruction. He will produce the data needed to train HyPER.

## Material
- [Custom Class Example](https://gitlab.cern.ch/dbaronmo/di-tau-trainer/-/tree/main/DiTauTrainer?ref_type=heads): provides examples of kinematic variables and how they can be used in a FastFrames custom class.
- [FastFrames Mini-Analysis tutorial](https://atlas-project-topreconstruction.web.cern.ch/fastframesdocumentation/latest/tutorial/#analysis-prototyping-with-cutflows-mini-analysis): to make the cutflow.
