---
layout: page
title: ""
---

## Dynamical structure of massive galaxies in cosmological simulation using machine learning

Individual galaxy can be divided into different components, e.g. halo, bugle (classical bulge + pseudo bulge) and disk (cold disk + warm disk). There are large differences shown in many quantities, e.g. angular momentum, binding energy, age, metallicity, etc., of these components due to their different formation history. However, it is hard to measure these quantities from observation because we can only get two dimensional information for the most of time. Therefore, we would like to explore the characteristics of these quantities of different components in massive galaxies by cosmological simulation IllustrisTNG. And we aim to create a dynamical template for these quantities of different components and apply it to observation.

Firstly, I selected massive galaxies in IllustrisTNG100. To decompose these galaxies into different components (halos, bulges, disks), I applied Gaussian Mixture Model to stellar particles of each galaxy using their angular momentum, binding energy, age and metallicity. Consistent with observational data, I found that most of massive galaxies are dominated by halos and bulges but there are still comparable number of disks. For each components, I did Principal Component Analysis to distribution function of these quantities. Using eigenvectors and PCs, I reconstructed and generated template distribution function for these quantities of each components. I shown differences among different components for the template of the same quantity.

This work is still ongoing. Next, I will use these templates to generate mock stellar particles and apply them to observational data.

