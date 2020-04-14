---
title: "SymAE: an autoencoder with embedded physical symmetries for passive time-lapse monitoring"
date: 2020-01-01
publishDate: 2020-01-17T02:43:54.254253Z
authors: ["Pawan Bharadwaj", "Matt Li", "Laurent Demanet"]
publication_types: ["1"]
abstract: "We introduce SymAE, an auto-encoder architecture that learns to separate multichannel passive-seismic datasets into qualitatively interpretable components: one component corresponds to path-specific effects associated with subsurface properties while the other component corresponds to the spectral signature
of the passive sources. This information is represented by two latent codes produced by our encoder. The novelty that enables SymAE to achieve this separation lies with the physical symmetries that are directly embedded into the architectural
design of the encoder. These symmetries impose that 1. the output of the source-specific encoder is indifferent to the ordering of the receivers; and 2. the output of the path-specific encoder is indifferent to the source signatures. Our numerical
experiments demonstrate that this is sufficient for achieving the intended separation.
The ability to qualitatively distinguish between source- and path-induced effects plays a critical role for time-lapse monitoring of visco-acoustic subsurface models where data is generated from induced passive seismic sources e.g., during CO2 injection
or hydraulic fracturing. Here the problem suffers from inherent ambiguities in whether the time-lapse changes in the data should be attributed to subsurface changes such as P-wave velocity, mass density, and seismic quality factor (i.e., path effects) or because of difficulties in physically-reproducing the source wavelet (i.e. source effects). SymAE resolves these ambiguities by construction and enables reliable subsurface monitoring in these settings. We provide numerical results to show that we can accurately detect changes arising from both effects."
featured: false
publication: "*SEG Technical Program Expanded Abstracts 2020*"
---

