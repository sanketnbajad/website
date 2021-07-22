---
title: Symmetric Autoencoder

summary: Redatuming physical systems to generate virtual experimental data.
tags:
- Deep Learning 
- Time-lapse Imaging
- Redatuming
- Physics-embedded Networks
- Virtual Data
date: "2020-10-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

draft: false

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
  preview_only: true

links:
- icon: external-link-alt
  icon_pack: fas
  name: Follow

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

{{< figure src="symae.png" title="Architecture of symmetric autoencoder.  The information that is coherent across the instances of a datapoint can only propagate through the network via solid arrows — notice the stochastic regularization employed to prevent its propagation. We used colored arrows to indicate the propagation of the remaining instance-specific nuisance information — notice that asymmetric function, i.e., symmetric w.r.t.  the order of the instances, prevents its propagation.  As a result, the autoencoder disentangles the coherent information from the nuisance variations in the latent space." numbered="true" lightbox="true" >}}

We proposed unsupervised deep-learning architecture called symmetric autoencoder (SymAE) to achieve
redatuming. The key idea is that SymAE learns to represent the measurements using a latent code, in which
the coherent and the nuisance information are disentangled. This unsupervised disentanglement is possible due
to the following characteristics of SymAE’s architecture.
* Physical symmetry is explicitly embedded into the encoder so that certain dimensions of the latent code are
invariant to the ordering of instances. This encoder prevents the communication of the instance-specific nuisance
variations, thereby purely encoding the coherent information. 
* The remaining latent-code dimensions are orthogonalized by stochastic regularization such that they
fail to represent coherent information. Therefore, these
latent components correspond only to the nuisance variations. 

The structuring mentioned above means that
the redatuming is equivalent to swapping the coherent
codes in the latent space before decoding into a virtual
instance. SymAE’s redatuming preserves and captures the salient features of
the underlying physical modeling operator, thus enabling the use of virtual datapoints for subsequent downstream
tasks such as parameter estimation.




