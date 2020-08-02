---
title: Redshift of Earthquakes

summary: A robust factorization of the teleseismic waveforms resulting from an earthquake.
tags:
- Seismology
- Blind Deconvolution 
- Rupture Characterization 
- Earthquake Spectrum
date: "2019-12-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
  preview_only: true

links:
# - icon: external-link-alt
  # icon_pack: fas
  # name: Follow
url_code: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"
# url_pdf: "https://ieeexplore.ieee.org/document/8680655"
# url_slides: "https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_FBD_slides_SEGAM.pdf"
# url_video: "https://www.youtube.com/watch?v=VLhvXITeFb0"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

{{< figure src="redshift_fig.png" title="Schematic of waves emitted due to a rupture propagating from west (azimuth $\theta=270^{\circ}$) to east (90$^{\circ}$). a) Blue waves emitted towards the east are shortened, while the red waves traveling towards the west are lengthened. These waves undergo complex scattering (squares) before they reach the receivers (triangles), resulting in a challenging source-spectrum estimation problem. b) I have developed a signal model to factorize the measurements, effectively removes the complex scattering or path effects and directly estimates the source spectra (red-blue graphs) at the receivers. The variability of the normalized source spectrum with $\theta$ can be used to infer the kinematic rupture parameters." numbered="true" lightbox="true">}}


<div style="text-align: justify">
The hazard assessment of earthquakes is closely related to the propagation of their associated ruptures. This research 
responds to numerous fundamental challenges involved in directly measuring source signals
that originate from a propagating rupture.
It is desirable to directly measure the source pulses 
at the seismometers and subsequently infer 
quantities that are related to the rupture propagation.
However, 
the signals measured in place of those pulses are affected by the subsurface properties through which they propagate
before reaching these stations.
Thus, instead of measuring the earthquake source signal directly, 
each seismic station records 
two types of information that are convoluted into a single signal: 
information about the earthquake (source pulse) and information about the 
unknown 
subsurface features through which
it passed (path effects).
The path effects may distort the earthquake source signal, for example,
due to:

 * one or more reflections off of geological layers in the subsurface; 
 * intrinsic attenuation of the porous-rock medium.
 
Consequently, an accurate characterization of the earthquake rupture 
involves reliably analyzing the recorded seismograms  to separate the path effects 
from the earthquake pulses.  Current methods for separating out the two types of information 
rely on dubious assumptions, and may be confounded because extracting source pulse 
requires assumptions about the path, but conversely
extracting path effects requires assumptions about the source. 
This research introduces to seismology a new analysis method, _focused blind deconvolution_ (FBD), 
that can be used to extract source or path information 
without relying on traditional assumptions. 
Instead, this method compares data from the same source picked up by multiple receivers, 
and uses advanced signal processing to identify similarities and differences among the data. 
Similarities among the signals can be identified as source effects, 
while dissimilarities indicate path effects. 
Because it does not require the aforementioned assumptions, 
this method will provide more accurate and reliable source information to seismologists. 
 </div>



{{< figure src="nicobar1_spec_compare.png" title="FBD factorizes the recorded spectra $|D|$, due to the Nicobar earthquake, into the source $|\hat{S}|$ and the path $|\hat{G}|$ at multiple azimuths. Note that the source spectrum exhibits frequency scaling, with higher corner frequency in the direction of the rupture propagation (indicated by an arrow) and vice versa." numbered="true" lightbox="true" >}}