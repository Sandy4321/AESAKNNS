# Continual Learning for Multi-Label Drifting Data Streams using Heterogeneous Ensemble of Self-Adjusting Nearest Neighbors

Multi-label data streams are among the most profound research areas in contemporary machine learning. Algorithms must be able to consider instances in real time with non-exclusive labels over possibly infinite, drifting streams. In this paper we propose a novel ensemble method for multi-label drifting streams named Heterogeneous Ensemble of Self-Adjusting Nearest Neighbors (HESAkNN). It leverages a self-adjusting kNN as a base classifier with the advantages of ensembles to adapt to concept drift in the multi-label environment. To promote diverse knowledge within the ensemble, each component classifier is given a unique set of features and samples to train on. These samples are distributed to classifiers in a probabilistic manner that follows a Poisson distribution. Accompanying these mechanisms, a collection of ADWIN detectors monitor each classifier for the occurrence of a concept drift. Upon detection, the algorithm automatically begins to train additional classifiers in the background to attempt to capture new concepts. After a pre-determined instance duration, both active and background classifiers are compared and only relevant concepts are selected to populate the new active ensemble. The experimental study compares the proposed approach with 30 other classifiers including problem transformation, algorithm adaptation, kNNs, and ensembles on 30 diverse multi-label datasets and 11 performance metrics. Results are validated using non-parametric statistical anaylsis.