---
layout: page
title: ""
---

## Photoheating feedback during reionization

[ADS link](https://ui.adsabs.harvard.edu/abs/2019MNRAS.488..419W/abstract)

This is the first fully self-consistent radiation-hydrodynamic simulation of reionization performed by Arepo-RT + Illustris galaxy formation model. We studied the back-reaction of reionization on galaxy formation, i.e. the effects of photoheating feedback. To isolate photoheating feedback and to examine how it couples with supernova (SN) feedback, we ran a bunch of simulations by turning radiative transfer or SN feedback on and off. We also ran simulations using the Faucher-Giguere+09 UV background. Our fiducial SN feedback + radiative transfer simulation finishes reionization at z=6. The plot below shows the star formation rate (SFR) - halo mass relations in different simulations. The upper panels show simulations with SN feedback. The UV background turns on at z&gt;10, so it acts like an early reionization. This can be mitigated by using a UV background with a more realistic IGM thermal history. What is surprising from this figure is that at z=6 when reionization finishes, there is only a small suppression of SFR at halo masses below 10<sup>8.4</sup> M<sub>&#8857;</sub>, contrary to previous works that find quenching of the &lt;10<sup>9</sup> M<sub>&#8857;</sub> halos at the end of reionization. The bottom panels, which shows simulations without SN feedback, indicate that the reason for this small suppression of SFR is that photoheating is weakened by SN feedback. This is actually a result of our non-local stellar feedback scheme: the wind particles do not have an impact on the dense ISM gas. In simulations with local SN feedback, photoheating and SN feedabck are expected to amplify the effects of each other on suppressing the SFR in low-mass halos.

{% include image.html url="SFR-Mhalo.png" alt="Whoops! See Fig.6 of my paper." description="SFR-halo mass relations in different simulations." %}

Fortunately, our finding that photoheating feedback is sub-dominant compared to SN feedback in regulating star formation is more robust. This is also found in other simulations or semi-analytic models. A consequence of this result (and that photoheating only affects the low-mass &#8818;10<sup>9</sup> M<sub>&#8857;</sub> halos) is that the faint-end slope of the high-z UV luminosity function may not be so sensitive to photoheating feedback that a flattening of the faint-end slope due to reionization is detectable. This is illustrated in the figure below, which again shows simulation with (upper panels) and without (lower panels) SN feedback. The resolution of our simulations only allows us to plot the UVLF to -15 mag, but there might be a small suppression of faint-end slope if we could plot to -14 mag, which roughly corresponds to halo mass of 10<sup>9</sup> M<sub>&#8857;</sub>.

{% include image.html url="UVLF.png" alt="Whoops! See Fig.7 of my paper." description="UV luminosity functions in different simulations." %}

