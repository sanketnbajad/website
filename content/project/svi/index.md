---
title: Super-virtual Interferometry 

summary: A denoising model for imaging seismic refractions and diffractions.
tags:
- Interferometry  
- Refraction Imaging
- Head-waves

date: "2014-11-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://pawbz.github.io/FocusedBlindDecon.jl/dev/"

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
  preview_only: true

links:
- icon: external-link-alt
  icon_pack: fas
  name: Journal
  url: "https://academic.oup.com/gji/article/188/1/263/633573"
url_slides: "https://github.com/pawbz/pawbz.github.io/blob/src/pdf/slides/Pawan_svi_cmb_compressed.pdf"
url_pdf: ""
url_video: ""


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

{{< figure src="svi_cmb_illustration.png" title=" Intermediate steps of denoising via super-virtual interferometry (SVI) for core-mantle boundary diffractions. Every iteration of SVI consists of a)---c) a cross-correlation and summation of the data to generate records with virtual arrivals, followed by  d)---f) a convolution of the records with the virtual arrivals to create records with super-virtual arrivals." numbered="true" lightbox="true" >}} 

<div style="text-align: justify">
In this project, I have established a novel physics-based 
denoising model for seismic refraction imaging.
It was carried out in close collaboration with marine geophysicists at The University of Texas at Austin and
King Abdullah University of Science and Technology. 
The experimental goal was to 
understand the sub-seafloor geology using refracted seismic energy from the 
geological boundaries.
Curstal-scale ocean-bottom-seismometer (OBS) surveys were carried out with sufficiently large
offset i.e.,
distance between the OBS stations and the airgun sources. Large offsets facilitate
the recording of the refracted signals radiated from deep geological boundaries, such as the 
MOHO.
However, as the energy propagates over large distances, the signal strength decays 
resulting in poor signal-to-noise ratio.
Consequently, an accurate tomography and imaging of the crustal structure required denoising
 of the refracted energy.


Signal processing methods based on seismic interferometry principally extract energy, which is 
_coherent_
across the source and/or receiver dimensions of the measurements.
However, the existing interferometric signal models were not reliable when focused on the application to 
seismic refractions.
I have identified a 
special coherent structure for the refracted waves in seismic data that led to a 
reliable interferometric model for denoising. 
This signal model boosted our groups efforts to perform denoising, 
and the subsequent algorithms resulted in a subfield 
of seismic interferometry that I spearheaded: 
super-virtual interferometry (SVI). 
SVI constructively stacks (sums up) refracted energy 
from hundreds of weak air-gun sources to 
enhance its signal-to-noise ratio.
My numerical experiments have shown that 
SVI can potentially boost 
the signal-to-noise ratio of the refracted seismic 
energy in the order of $\sqrt{N}$, where $N$ is the number of intermediate 
stations between a given source and receivers pair.
Furthermore, I have also demonstrated the benefits of SVI for a variety of 
seismic surveys including near-surface geophysical experiments that image bedrock.
In all these experiments, without SVI nearly half of the measured large-offset measurements 
was unusable for refraction traveltime tomography.
Later on, I have developed a similar interferometric signal model for denoising
core-mantle boundary (CMB) diffractions in
collaboration with seismologists. 
This signal model for CMB diffractions, along
with an intuitive sketch of SVI, 
is depicted in figure above.

 </div>



