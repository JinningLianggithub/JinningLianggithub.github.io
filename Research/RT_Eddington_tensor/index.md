---
layout: page
title: ""
---

## Accuracy of moment-based radiative methods on simulating reionization

[ADS link](https://ui.adsabs.harvard.edu/abs/2021JCAP...02..042W/abstract)

Simulating the reionization process requires performing radiative transfer, which is expensive in terms of both computing time and memory consumption.  By taking the angular moments of the radiative transfer equation and closing at the quadrupole order, the moment-based radiative transfer methods greatly reduces the computational cost and has become one of the most popular tool for simulating reionization.  However, the accuracy of the closure methods (Eddington tensors) used to close the set of moment equations on simulating the reionization observables has not been studied in detail before.  Since most of the observational constraints on reionization still come from the post-reionization Lyamn-&alpha; forest, in this work we examine the accuracy of two common Eddington tensors choices, M1 and OTVET, on simulating the post-reionization observables related to the forest.

We designed two toy problems to mimic the physical state of the post-reionization IGM.  In the first toy problem, we studied the ionization structure of a spherical absorber with a monomial density profile with uniform radiation coming from infinity.  This mimics the situation of self-shielding absorbers of ionizing photons (Lyman-limit systems) after reionization, which limit the photon mean free path and set the metagalactic photoionization rate.  The tens of comoving Mpc photon mean free pathafter reionization indicates roughly uniform ionizing background.  We found that if radiation follows the moment equations closed by M1 and OTVET, there is twice more photon flux going into the absorber compared to the case where radiation behaves as rays, resulting in M1 and OTVET over-ionize the absorber (see figure below).  This leads to increased recombination rates and hence 30-40% higher required photon emissivity to balance the recombinations.  The use of moment-based radiative transfer methods thus likely bias the calibration of the simulations, which uses the post-reionization metagalactic photoionization rate, photon mean free path, etc. obtained from the Lyman-&alpha; forest transmissions.

{% include image.html url="absorberprofiles.png" alt="Whoops! See Fig.2 of my paper." description="M1 and OTVET over-ionize absorbers of ionizing photons in simulations of reionization." %}

In the second toy problem, we used perturbation theory calculations to study fluctuations in the post-reionization ionizing background, which have been a successful scenario in explaining the observed large-scale fluctuations in the Lyman-&alpha; forest transmissions.  We found that the M1 Eddington tensor reduces to being isotropic at linear order in density, leading to drastically underestimated fluctuations in the ionizing background on scales below the photon mean free path (see figure below).  Predictions by OTVET, on the other hand, depend on the adopted box size of the simulations.  OTVET reduces to being isotropic in the case of very large box owing to the Olber's paradox and results in underpredicted ionizing background fluctuations, but becomes more anisotropic than the exact solution if the box size is smaller than a photon mean free path, leading to overpredicted ionizing background fluctuations.  The moment-based radiative transfer method thus likely bias the simulated fluctuations in the Lyman-&alpha; forest transmissions on 50 Mpc/h scales.

{% include image.html url="Gammapowerspec.png" alt="Whoops! See Fig.3 of my paper." description="M1 and OTVET bias the simulated fluctuations in the post-reionization ionizing background." %}

Unfortunately, we do not have a method to resolve the above issues related to the moment-based methods, and we have also found that short-characteristics ray-tracing methods or closing the moment equations at higher orders do not necessarily simulate the ionizing background fluctuations a lot more accurately.

