---
layout: page
title: ""
---

## Accuracy of moment-based radiative methods on simulating reionization

[ADS link](https://ui.adsabs.harvard.edu/abs/2021JCAP...02..042W/abstract)

Most reionization simulations use the moment-based radiative transfer algorithm which introduces unphysical assumptions about the radiation field. These assumptions significantly lower the computational cost but likely cause errors when simulating the post-reionization IGM. While simulations aim to match the Lyman-alpha forest observations, the accuracy of approximate radiative transfer methods has not been studied in detail.

I performed a pen-and-paper calculation of the radiative transfer equation to estimate how the approximate numerical algorithms would err in simulating the post-reionization IGM by designing toy problems mimicking the IGM. I found that moment-based methods over-ionize absorbers of ionizing photons, increasing the required emissivity by &sim;30% to balance the higher recombination rate (Fig. 1). I thus showed that reionization simulations are unlikely to match the observed photoionization rate, emissivity, and photon mean free path at the same time. I also found that moment-based algorithms can bias the post-reionization ionizing background fluctuations by tens of percent, while ionizing background fluctuations are the most likely scenario to explain the observed large scatter in the Lyman-alpha forest flux (Fig. 2). As the first one to prove that reionization simulations can significantly bias the level of fluctuations in the simulated Lyman-alpha forest flux, my work acts as a significant warning to the simulation community.

{% include image.html url="absorberprofiles.png" alt="Whoops! See Fig.2 of my paper." description="Fig. 1: M1 and OTVET algorithms over-ionize absorbers of ionizing photons in simulations of reionization." %}

{% include image.html url="Gammapowerspec.png" alt="Whoops! See Fig.3 of my paper." description="Fig. 2: M1 and OTVET algorithms bias the simulated fluctuations in the post-reionization ionizing background." %}

Unfortunately, we do not have a method to resolve the above issues related to the moment-based methods, and we have also found that short-characteristics ray-tracing methods or closing the moment equations at higher orders do not necessarily simulate the ionizing background fluctuations a lot more accurately.

