---
layout: page
title: ""
---

## Photometric properties of reionization-epoch galaxies in the Simba simulations

[ADS link](https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.5636W/abstract)

Studying galaxies at z&#8819;6 has been one of the frontiers of observational and theoretical research. Matching the properties of these distant objects is a basic goal of galaxy formation simulations, and conversely simulations can be used to make predictions for future observations. In this work we examined the photometric properties of z=6-8 galaxies in the [Simba](https://ui.adsabs.harvard.edu/abs/2019MNRAS.486.2827D/abstract) simulations, specifically the 25 h<sup>-1</sup>Mpc and 50 h<sup>-1</sup>Mpc boxes.

We focused on the three observables extensively explored in the literature that describe the global properties of z&#8819;6 galaxies: the UV luminosity function (UVLF), the UV continuum slope (&beta;) - UV luminosity (M<sub>1500</sub>) relation, and galaxy sizes and morphologies. Mock photometry and image generation are performed with [pyloser](https://pyloser.readthedocs.io/en/latest/). We explored three different dust extinction laws: [Salmon16](https://ui.adsabs.harvard.edu/abs/2016ApJ...827...20S/abstract), [Calzetti00](https://ui.adsabs.harvard.edu/abs/2000ApJ...533..682C/abstract), and [SMC](https://ui.adsabs.harvard.edu/abs/2003ApJ...594..279G/abstract).

The plot below summarizes the comparison of the simulations to observations at z=6. Top panels show the UVLF (left) and &beta;-M<sub>1500</sub> relations (right) assuming different dust extinction laws, combined from the two simulations. Overall, Simba roughly matches the observations, and the Calzetti law provides the overall best match to observations. We therefore moved on to generating mock images using only the Calzetti law. The bottom panel shows the rest-UV size-luminosity relations measured with three different methods, where in the growth curve method (left) and Sersic fit method (middle) mimic the size measurements in observational studies, and the 3D half-light radii (right) can be seen as the true size of the simulated galaxies. Again, Simba is able to match the observations.

<figure>
  <img src="UVLF_and_beta.png" alt="Whoops! See Fig.4 and 5 of my paper." width="100%">
  <img src="size-lum.png" alt="Whoops! See Fig.9 of my paper." width="95%">
  <figcaption>The simulated z=6 UVLF (top left), &beta;-M<sub>1500</sub> relations (top right) assuming different extinction laws, and the rest-UV size-luminosity relations (bottom) with the galaxy size measured with three different methods.</figcaption>
</figure>

With Simba being able to match the observations, we are able to make predictions for future JWST observations. We explored the rest-optical sizes of the simulated z=6 galaxies, which will be observable with JWST, and found that there is a surprising one-to-one relationship with the rest-UV sizes. We also examined how the observed half-light sizes trace the 3D half-stellar mass sizes. What might be more interesting is that Simba predicts very early metal enrichment, and so the z=8 UVLF appears a bit low compared to observations (see figure below). This may be contradictory to a number of previous works, but the early metal enrichment manages to yield good matches to the observations at z=6. Whether the z&ge;6 galaxies experience early metal enrighment will be testable with JWST.

<figure>
  <img src="z8.png" alt="Whoops! See Fig.4 and 7 of my paper." width="100%">
  <figcaption>The simulated z=8 UVLF (left) and gas-phase mass-metallicity relations at z=6 and 8 (right), which are actually higher than the z=2 observations.</figcaption>
</figure>

Finally, this paper is a show-off of pyloser and our image generation routine. The plot below shows the mock HST (top panels) and JWST (bottom panels) images of a simulated galaxy in Simba, without PSF and noise. The comparison is dramatic.

<figure>
  <img src="mock_images.png" alt="Whoops! See Fig.1 of my paper." width="100%">
  <figcaption>Mock HST and JWST images of a simulated galaxy in Simba, without PSF or noise effects.</figcaption>
</figure>

