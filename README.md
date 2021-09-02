# [Higgs Boson Machine Learning Challenge](https://www.kaggle.com/c/higgs-boson)

Discovery of the long awaited Higgs boson was announced July 4, 2012 and confirmed six months later. 2013 saw a number of prestigious awards, including a Nobel prize. But for physicists, the discovery of a new particle means the beginning of a long and difficult quest to measure its characteristics and determine if it fits the current model of nature.

A key property of any particle is how often it decays into other particles. ATLAS is a particle physics experiment taking place at the Large Hadron Collider at CERN that searches for new particles and processes using head-on collisions of protons of extraordinarily high energy. The ATLAS experiment has recently observed a signal of the Higgs boson decaying into two tau particles, but this decay is a small signal buried in background noise. 

The goal of the Higgs Boson Machine Learning Challenge is to explore the potential of advanced machine learning methods to improve the discovery significance of the experiment. No knowledge of particle physics is required. Using simulated data with features characterizing events detected by ATLAS, your task is to classify events into "tau tau decay of a Higgs boson" versus "background." 

## File descriptions

- training.csv - Training set of 250000 events, with an ID column, 30 feature columns, a weight column and a label column.
- test.csv - Test set of 550000 events with an ID column and 30 feature columns.

For detailed information on the semantics of the features, labels, and weights, see the technical documentation from the LAL website on the task.

Some details to get started:

- all variables are floating point, except PRI_jet_num which is integer
- variables prefixed with PRI (for PRImitives) are “raw” quantities about the bunch collision as measured by the detector.
- variables prefixed with DER (for DERived) are quantities computed from the primitive features, which were selected by  the physicists of ATLAS
- it can happen that for some entries some variables are meaningless or cannot be computed; in this case, their value is −999.0, which is outside the normal range of all variables
