---
title: "SymAE: redatuming timelapse data to create virtual baseline sources in the monitoring medium"
date: 2020-12-01
publishDate: 2020-01-17T02:43:54.253708Z
authors: ["Pawan Bharadwaj", "Matt Li", "Laurent Demanet"]
publication_types: ["1"]
abstract: "We introduce an auto-encoder called SymAE that learns to redatum time-lapse data recorded in passive-seismic subsurface-monitoring experiments. SymAE analyzes the baseline and monitor records and creates new monitor records that behave as if the virtual baseline sources were active in the monitoring medium. No explicit modeling is required for this redatuming as SymAE can automatically extract both the baseline sources and the monitoring medium from large amounts of passive-seismic data. As a result, differences between the virtual and actual baseline-source records primarily contain only about the subsurface time-lapse changes with minimal pollution from the variability in passive-source characteristics such as e.g., location, signature, radiation pattern, direction-of-arrival in case of incoming planewaves etc. This is an essential first step towards realistic passive timelapse analysis as it overcomes the requirement of stationary passive sources, which currently limits conventional interferometric processing.
SymAE is trained to represent passive seismic data using two separate latent codes produced by its encoder. The first latent code represents the similarity or coherency among multiple instances of passive data; therefore it is associated with the path-specific effects. The second latent code represents the remaining dissimilarities; therefore it can be associated with information that varies among the passive sources. Finally, the above-mentioned virtual records can be created by mixing latent codes of seismic records — a demo is given in the figure attached."
featured: false
publication: "*Proceedings of the 2020 Fall Meeting AGU*"
---

