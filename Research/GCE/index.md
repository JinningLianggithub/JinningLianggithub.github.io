---
layout: page
title: ""
---

## Galaxy Chemical Evolution

[Paper preview](/../files/Yields_NuPyCEE.pdf)

At the beginning of the universe, there were only H, He, and small amounts of Li. The first stars formed from these elements and began to fuse them into heavier elements like C, N, and O. As these stars evolved and eventually exploded they dispersed these heavier elements into the surrounding gas and dust, enriching it with new elements. Over time, subsequent generations of stars formed from this enriched gas, incorporating even more heavy elements into their composition. As galaxies continue to evolve and merge, the chemical composition of their stars and gas mix and become more complex. 

However, there are many uncertain process in galaxy chemical evolution. Stellar yields is one of them due to the lack of understanding and observational data for massive stars. The differences in stellar yields for 12 elements can be seen in Fig.1. To explore the uncertainty in different stellar yields, compare and show their difference, I ran fixed Milky-Way-like parametrization of NuPyCEE simulation with stellar yields as the only variable. To explain the scatter existed in stellar abundance especially in halo stars, I grouped the yields by their physical process and test if yield combinations match data scatter and standard deviation. I defined criteria that estimate whether an element is in agreement with the data, or if the model overestimates or underestimates it in various metallicity bins. The summary for the criteria can be seen in Fig.2. Then I used the criteria to explore he statistical properties spanned by such yields. I found the differences and commonalities among yield sets and found the scatter of the abundance
data is inconsistent with a scatter resulting from averaging runs across yield prescriptions.

{% include image.html url="comparison.png" alt="See Fig.1 of my paper." description="Fig. 1: Logarithmic mass-fraction of the returned yields for 12 elements at solar metallicity, as a function of logarithmic stellar mass. The 'shift' label indicates the factor by which the mass-fractions have been shifted. The legends for different stellar yields can be seen in the paper." %}

{% include image.html url="piechart.png" alt="See Fig.17 of my paper." description="Fig. 2: For each of Group A, B, and C, the summary of the Judgement criteria (Median, standard deviation, and scatter) for the four metallicity bins. Details can be seen in the paper." %}

I have also joined GalCEM (GALactic Chemical Evolution Model) collaboration and provide nearly all abundance ratio data we need. One can see it from [ADS link](https://ui.adsabs.harvard.edu/abs/2023ApJS..264...44G/abstract)It's a user-friendly detailed, and modular, one-zone GCE model. In the future, I will use this model to explore many interesting things such as parameter space in GalCEM, galaxy cluster enrichment by galaxy outflow, etc.