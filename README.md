# Quark Matter 2015 poster

Source for my [Quark Matter 2015 poster](https://indico.cern.ch/event/355454/session/33/contribution/331/attachments/1160023/1669679/poster.pdf).

- `data/exp` contains experimental data tables from [hepdata](http://hepdata.cedar.ac.uk) and a `preprocess` script to convert them all to HDF5.
- `data/model` contains scripts for use with [heavy-ion-collisions-osg](https://github.com/jbernhard/heavy-ion-collisions-osg):
  - `make-design` generates a Latin-hypercube design and corresponding input files for the OSG workflow
  - `compute-event-observables` postprocesses event-by-event particle data into observables such as identified particle yields, Qn vectors, etc.
  - `compute-batch-observables` takes the computed event observables and further postprocesses them into centrality-dependent observables such as average particle yields, flow cumulants, etc.
- `calibration/calibrate` runs MCMC and generates posterior distributions for the model parameters using my library [mtd](https://github.com/jbernhard/mtd).
- `poster.svg` is the Inkscape file.
