---
layout: page
title: ""
---

## A non-parametric Lagrangian halo biasing model

[Paper I](https://ui.adsabs.harvard.edu/abs/2022JCAP...02..002W/abstract)

[Paper II](https://ui.adsabs.harvard.edu/abs/2022arXiv221208095W/abstract)

Halos are traditionally assumed to be biased tracers of the large-scale structure, and their clustering can be modeled as a polynomial of the matter density field with a few unknown bias coefficients. However, the much rarer and more highly biased nature of reionization-epoch halos indicates a regime where this bias expansion method likely fails significantly. For instance, it may predict a negative number of halos or a sizable amount of halos in underdense regions.

As the first attempt ever to jump out of the traditional bias expansion framework, I developed a novel non-parametric halo biasing model and tested it using the well-studied z=0.5 halos in the AbacusSummit simulations. I obtained a non-parametric function that describes how many halos a given patch in the initial space should form, and found that this function deviates significantly from a polynomial of the matter density. More biased halos observe larger deviations, and my non-parametric model can outperform the bias expansion at recovering the halo power spectrum.

In the second paper, we extended our previous analytic formalism to training neural nets to obtain the non-parametric halo-to-mass ratio.  A NN allows us to include a much larger dimension of the input feature space than our initial least-squares approach.  We found that owing to the correlations of the input features at different smoothing scales, the halo-to-mass ratio can be well described by only two directions in the original feature space.  We also found that 3 or more smoothing scales are needed to best recover the final halo field, while traditional bias expansion approach only uses 1 smoothing scale.  Our formalism will be most fruitful when studying high-redshift galaxies (e.g. z=2 Lyman-alpha emitters), a regime where traditional bias expansion is likely to fail.

{% include image.html url="illustration.png" alt="Whoops! See Fig.1 of my papers." description="An illustration of how we train the neural net to obtain the non-parametric halo-to-mass ratio (the f function)." %}

