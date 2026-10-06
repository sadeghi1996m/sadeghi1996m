---
title: "Research"
permalink: /research/
excerpt: "Spectral methods for graph signals, sensor placement under uncertainty, and EEG electrode placement for brain–computer interfaces."
---

My research studies how the structure of signals and measurement systems can guide reliable signal recovery. During my PhD, I worked on the following connected topics.

## Blind separation of graph signals

Graph signal processing uses relationships between observations to model and analyze data on networks. My early doctoral work examined the graph decorrelation (GraDe) algorithm for recovering latent graph signals from observed mixtures.

We identified a limitation caused by dominant eigenvalues in the graph spectrum: sample graph autocovariance matrices can deviate from the diagonal structure needed for effective separation. We developed an improved GraDe method that suppresses the contribution of these spectral outliers, improving separation for several graph models.

**Related paper:** [An improved GraDe method for blind separation of graph signals](https://doi.org/10.1109/TSP.2023.3331264), *IEEE Transactions on Signal Processing*, 2023.

## Sensor placement under uncertainty

Where should sensors be placed to recover the signals of interest from noisy measurements? I developed a statistical framework that models source-to-sensor gains using Gaussian processes, allowing uncertainty and prior knowledge to enter the placement problem.

The framework uses mean squared error and signal-to-interference-plus-noise ratio criteria, with stochastic optimization to find informative sensor locations. I also investigated sensor placement for sparse signal reconstruction in underdetermined systems, where both measurement noise and the properties of the sensing matrix influence recovery.

**Related work:** [Signal Processing, 2025](https://doi.org/10.1016/j.sigpro.2024.109659) · [EUSIPCO, 2023](https://doi.org/10.23919/EUSIPCO58844.2023.10289756) · [Manuscript under review]({{ '/publications/#under-review' | relative_url }}).

## EEG and brain–computer interfaces

I applied this framework to electrode placement for P300-based brain–computer interfaces. The aim is to select useful electrode locations while accounting for variability between people and reducing calibration requirements.

Our subject-independent electrode placement method learns common spatial patterns across a population. A hybrid method combines this prior knowledge with available recordings from a new participant through a Bayesian update.

**Related paper:** [Prior knowledge-driven robust electrode placement method for P300-based brain-computer interfaces](https://doi.org/10.1016/j.bspc.2026.110123), *Biomedical Signal Processing and Control*, 2026.

## Future directions

I am interested in graph machine learning, geometric deep learning, and statistical inference on graphs, particularly in how structural information and uncertainty can improve learning from complex signals.
