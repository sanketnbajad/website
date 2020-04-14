---
title: Blind Source Separation

summary: Data-driven Green's function retrieval from the multi-channel seismic data of a noisy source.
tags:
- Blind Source Separation 
- Independent Component Analysis 
- Deblending
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

image:
  caption:
  focal_point: TopRight
  preview_only: True

links:
- icon: external-link-alt
  icon_pack: fas
  name: Journal
  url: https://library.seg.org/doi/abs/10.1190/segam2017-17677817.1
- icon: external-link-alt
  icon_pack: fas
  name: Slides
  url: https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_Seismic_ICA_Tue_Talk.pdf

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
{{< figure src="featured.png" title="The receivers (r1 and r2) record the blended wavefield due to simultaneous random sources (red s1 and blue s2). ICA decomposes the wavefield into isolated records involving one source at a time. The deblended records at the first receiver are shown." numbered="true" lightbox="true" >}}

* This project demonstrates the application of frequency-domain independent component analysis to deblend random seismic sources. 
* ICA uses higher-order statistics to measure the Gaussianity of signals and working with convolutive mixtures (as in seismic exploration) is a challenging problem.




