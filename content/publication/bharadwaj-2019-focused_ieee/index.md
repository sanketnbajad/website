---
title: "Focused blind deconvolution"
date: 2019-01-01
publishDate: 2020-01-17T02:43:54.254808Z
authors: ["Pawan Bharadwaj", "Laurent Demanet", "Aimé Fournier"]
publication_types: ["2"]
abstract: "We introduce a novel multichannel blind deconvolution (BD) method that extracts sparse and front-loaded impulse responses from the channel outputs, i.e., their convolutions with a single arbitrary source. Unlike most prior work on BD, a crucial feature of this formulation is that it does not encode support restrictions on the unknowns, except for fixing their duration lengths. The indeterminacy inherent to BD, which is difficult to resolve with a traditional l1 penalty on the impulse responses, is resolved in our method because it seeks a first approximation where the impulse responses are: “maximally white” over frequency-encoded as the energy focusing near zero lag of the impulse-response temporal autocorrelations; and “maximally front-loaded”-encoded as the energy focusing near zero time of the impulse responses. Hence, we call the method focused BD (FBD). It partitions BD into two separate optimization problems and uses the focusing constraints in succession. The respective constraints in both these problems are removed as the iterations progress. A multichannel BD problem whose physics calls for sparse and front-loaded impulse responses arises in seismic inversion, where the impulse responses are the Green's function evaluations at different receiver locations, and the operation of a drill bit inputs the noisy and correlated source signature into the subsurface. We demonstrate the benefits of FBD using seismic-while-drilling numerical experiments, where the noisy data recorded at the receivers are hard to interpret, but FBD can provide the processing essential to separate the drill-bit (source) signature from the interpretable Green's function."
featured: true
publication: "*IEEE Transactions on Signal Processing*"
---

