---
title: Focused Blind Deconvolution

summary: Data-driven Green's function retrieval from the multi-channel seismic data of a noisy source.
tags:
- Blind Deconvolution
- Green's Function Retrieval 
- Focusing Constraints
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

image:
  caption: Marmousi experiment, where FBD (data panel 3) outperforms the conventional Green's function retrieval from noise (data panel 1) through cross-correlation (data panel 4). When compared to the true Green's function (data panel 2), note that FBD not only recovers the direct arrival but also the scattered arrivals due to the reflectors in the medium. 
  focal_point: TopRight
  preview_only: true

links:
- icon: external-link-alt
  icon_pack: fas
  name: Follow
  url: https://erlweb.mit.edu/announcements/robust-extraction-useful-information-seismic-measurements
- icon: external-link-alt
  icon_pack: fas
  name: Patent
  url: https://patents.google.com/patent/US20190349223A1/en
- icon: external-link-alt
  icon_pack: fas
  name: Slides
  url: https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_FBD_slides_SEGAM.pdf
url_code: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"
url_pdf: "https://ieeexplore.ieee.org/document/8680655"
url_slides: "https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_FBD_slides_SEGAM.pdf"
url_video: "https://www.pathlms.com/siam/courses/11267/sections/14660/video_presentations/128895"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
{{< figure src="FBD_movie2.png" title="Marmousi experiment, where FBD (data panel 3) outperforms the conventional Green's function retrieval from noise (data panel 1) through cross-correlation (data panel 4). When compared to the true Green's function (data panel 2), note that FBD not only recovers the direct arrival but also the scattered arrivals due to the reflectors in the medium." numbered="true" lightbox="true" >}}

* This research 
introduces an idea (focusing) that is important to 
resolve the indeterminacy inherent to multichannel blind deconvolution.
* FBD is a deconvolution algorithm that 
extracts sparse and front-loaded impulse responses from the channel outputs, i.e., 
their convolutions with a single arbitrary source. 
* This project also employs FBD to solve essential problems in both exploration and earthquake seismology.
In this context, FBD not only 
outputs the subsurface Green's function, which can be directly input to imaging, 
but also helps us understand the noisy source characteristics.


{{< figure src="FBD_movie1.png" title="Info-graphic of focused blind deconvolution, which is a data-driven Green's function retrieval algorithm for multi-channel seismic data of a noisy source." numbered="true" lightbox="true" >}}




