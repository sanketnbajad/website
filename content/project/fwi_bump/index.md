---
title: Multi-objective Full Waveform Inversion 

summary: When the seismic waveforms are too complicated to be analyzed during inversion, a simplification of them into envelope-like bumpy waveforms can be useful.

tags:
- Imaging
- Full Waveform Inversion
- Multi-objective Optimization
- Velocity Model Building
- Bump Functional
- Cycle Skipping

date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
  preview_only: true

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/bharadwajpawan
- icon: external-link-alt
  icon_pack: fas
  name: Slides
  url: https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_BumpFunctional_Slides.pdf
- icon: external-link-alt
  icon_pack: fas
  name: Slides
  url: https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_SEG13slides.pdf
- icon: external-link-alt
  icon_pack: fas
  name: Journal
  url: https://academic.oup.com/gji/article/206/2/1076/2605991
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

{{< figure src="marm_bump.svg.png" title="Subsurface P-wave velocity models. a) True. b) FWI result using the least-squares objective — convergence to local minima. c) Multi-objective FWI with the auxiliary bump functional." numbered="true" lightbox="true" >}}


### Cycle Skipping in Full Waveform Inversion (FWI)
"When the seismic waveforms are too complicated to be analyzed during inversion, a simplification of them into envelope-like bumpy waveforms can be useful."

* This research formulates a bump functional that computes the data misfit in seismic inversion
after a simplification. 
* A multi-objective FWI strategy, where the bump functional is 
used as an auxiliary functional to overcome the well-known cycle-skipping problem, is proposed.
* Advantages of seismic inversion that maximizes the correlation between the observed and modelled seismic data.



### Multi-parameter Seismic Inversion

An analysis of the multi-parameter inverse problem in quantitative seismic imaging.
[\[slides\]](https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_EAGE14slides.pdf) 
[\[paper\]](https://arxiv.org/abs/1804.01184)

