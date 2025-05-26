---
title: How to use rattling
description: ""
summary: ""
date: 2024-12-04T18:53:05-06:00
lastmod: 2024-12-04T18:53:05-06:00
draft: false
weight: 40
math: true
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
author: Pavel Chvykov
---
Q: So what exactly can Rattling theory tell me for my specific system, experiment or question? How do I use it?

First you need to consider if you think the Rattling hypothesis should hold in your system. Generally, it should hold for ["typical"](/docs/background/typicality/) systems (see [these guidelines](/docs/background/typicality/#general-guidelines)). If this applies, then there are several things you can do.

## Predict relative likelihoods 

To get the steady-state probability of any system configuration $x$, you need to know its Rattling $\mathcal{R}(x)$ and the normalization $Z$ (just as with Boltzmann distribution):
$$p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}/Z$$
Rattling is powerful because it is easy to measure $\mathcal{R}(x)$—one just needs to initialize the system in state $x$ and see how fast it leaves that state on average. The generalization for systems with continuous configuration space is $\mathcal{R}(x) = \frac{1}{2} \log \det D(x)$, where $D(x)$ is the effective diffusion tensor at $x$, which can be similarly approximated from how fast it leaves $x$ (from taking a few short system trajectories starting at $x$, and calculating the covariance matrix (see details in [our Science paper](https://www.science.org/doi/10.1126/science.abc6182) Materials and Methods, sec 3.2). 
Note that, empirically, it is easier to measure Rattling of a state than it is to measure energy of a state, since energy cannot be locally defined in terms of transition rates among the states.

Without knowing $Z$, this allows us to predict relative likelihoods:
$$\frac{p_{ss}(x)}{p_{ss}(y)} \approx e^{-\gamma \,\left[\mathcal{R}(x) - \mathcal{R}(y)\right]} $$
The coefficient $\gamma$ here is a system-specific constant, which will often be close to 1, but may deviate somewhat if the system doesn't quite meet the mentioned [guidelines](/docs/background/typicality/#general-guidelines) (e.g., its configuration space is 6-dimensional rather than 100-dimensional). See [here](/docs/background/formalizing-rattling/) for more details on what $\gamma$ is. Either way, it is easy to estimate empirically from a few state-measurements and then make predictions for the rest. 

## Predict absolute likelihoods?

But to predict whether of not a system will self-organize, relative likelihoods are not enough, and so we need to find $Z$. $Z$, however, is not so easy to estimate empirically, since it depends globally on all configurations $x$. Unless we have empirical access to all system states, which is usually impractical, we need some theoretical calculation to find $Z$, and so some theoretical understanding of the global system properties. This is similar to finding the partition function in statistical mechanics, except that calculating energy of a state is well-known, while calculating its rattling is generally an [open question](/docs/research-directions/predicting-rattling/). 

We have some examples where we were able to successfully do this and predict the phase transition to self-organization (e.g., [Vicsek model](/docs/examples/vicsek-model/)), but it's not clear for which systems this is or isn't possible. 
In other cases, it may be possible to combine theoretical and empirical methods to estimate $Z$—by sampling a representative set of configurations and measuring their rattling (here you need a sufficient understanding of your system to know how to choose that "representative set").

## Destabilize by adding noise

## Predict self-organized configurations

## Control self-organized configurations 


([our paper](https://www.science.org/doi/10.1126/science.abc6182) examples - prop ratios, control, predict, etc...