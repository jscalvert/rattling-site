---
title: Typicality
description: ""
summary: ""
date: 2024-12-04T18:53:05-06:00
lastmod: 2024-12-04T18:53:05-06:00
draft: false
math: true
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
author: Pavel Chvykov
weight: 17
---
We claim that the Rattling hypothesis holds (i.e., predicts steady-state probability) for "typical" dynamical systems. On the one hand, "typical" here expresses an uncontrolled approximation – for a given system, it may be hard to determine a-priori how well Rattling will hold. On the other hand, it points to the intuition that Rattling should hold most of the time in real-world scenarios. 

## So what does "typical" mean exactly? 

Here we are referring to the concept of *typicality* – a related set of ideas and results that emerged over the last 50 years. Pankaj Mehta described it nicely in his [2024 paper "Theory is dead. Long live theory! For a 21st century statistical physics of life"](https://arxiv.org/pdf/2410.20506):

>Wigner showed that the statistical structure of nuclear resonances in the Uranium atom could be reproduced by modeling the Hamiltonian as a large symmetric random matrix.[^1] Winger’s conjectured that when a system becomes complex enough, many of its statistical properties will be “typical” and indistinguishable from a large random system subject to the same physical constraints as the object of study (i.e. is drawn from the same ensemble). In the case of Uranium, the relevant physical constraint Wigner identified was unitarity, which is why he considered symmetric random matrices to model the Hamiltonian of Uranium. More recently, this line of thinking has found great success in condensed matter theory in the context of Eigenstate Thermalization Hypothesis, which uses typicality to explain why even a single eigenstate of a sufficiently large manybody quantum system can be accurately described by statistical mechanics.[^2]
>
>As Freeman Dyson explained, this is a fundamentally “new kind of statistical mechanics, in which we renounce exact knowledge not of the state of a system, but the nature of the system itself.”[^3] What is nice about this approach is that it suggests a natural framework for thinking about living systems. Because it is agnostic to the origin of the constraints, it does not matter whether the relevant constraints originate from physical conservation laws, dynamics, geometry, energetics, evolutionary history, or even from specialized biological functions. For this reason, these ideas offer a promising avenue for thinking about how to model complex biological systems.
>
>In the last few years this program has been successfully applied to understand many properties of complex microbial communities, suggesting that it can be operationalized to gain biological insights[^4]. Moreover, modern generative models of proteins also naturally fall into this rubric. When stripped of all their bells and whistles, generative models of proteins are probabilistic models for sequence generation that respect the evolutionary and functional constrains embodied in amino acid conservation patterns.[^5]

This is also the essence of "maximum entropy (MaxEnt) modeling" – where in the absence of having detailed measurements of the system parameters, we assume these to take their most likely values, constrained by some macroscopic or global parameters that we can measure. This technique has been applied in many systems, and even works to model [neuron firing statistics](https://www.nature.com/articles/s41598-024-55922-9) and even [neuron connectivity](https://www.nature.com/articles/s41598-022-13674-4). In fact, MaxEnt is one way to derive the Boltzmann distribution, as well as our Rattling hypothesis (see Sec.2.2 in Supplement of [our paper](https://www.science.org/doi/10.1126/science.abc6182)).

## Adversarial fine-tuning

The main intuition behind "typicality" is that the system is large, complex, and did not suffer any adversarial fine-tuning. This is reminiscent of how a Neural Network can perfectly classify all "typical" cat images, unless someone adjusts the pixels slightly just right, so as to make it think it's a dog ([see here](https://medium.com/@wanguiwawerub/adversarial-attacks-on-neural-networks-240a47c76f4c)). In our case, such adversarial fine-tuning need not come from a malevolent agent, but from some pre-existing selection pressures. E.g., a biological organism is not a "typical" dynamical system as it has been fine-tuned by evolution. A pendulum is not a "typical" dynamical system because it's too simple. A crystal is not because it's too ordered (not complex enough). 


-------
So with this, [the question](/core-questions/#typicality-of-rattling) arises: how typical exactly are dynamical systems where Rattling hypothesis holds? Can we construct a random ensemble representing all real-world dynamical systems, and then see what's the probability of Rattling-friendly systems?

## General guidelines

While we cannot yet give rigorous [*a priori* test](/core-questions/#a-priori-test-of-rattling) that will tell us if Rattling hypothesis will hold, we generally expect it to hold for systems that:
1) have many interacting degrees of freedom
2) have no particularly strong symmetries. 
	This includes linearity, conservation of energy, etc. – as these could make the system act as a low-dimensional one or become integrable), and finally 
3) are in no way fine-tuned (such as by selection or evolution). 
	Note since Rattling is most interesting for explaining self-organization, such self-organized configurations or dynamics will necessarily be selected and fine-tuned. So one must distinguish the dynamical system itself from the specific behaviors that it might exhibit – and so this requirement is for the former. More subtle point here is that in some systems self-organization may happen in stages or hierarchically, in which case some sub-space of the dynamics remains "typical," while other degrees of freedom are fine-tuned. This scenario should still work with Rattling, but the details are an [open question](/core-questions/#hierarchical-self-organization).




[^1]:Wigner, Eugene P. "Random matrices in physics." SIAM review 9.1 (1967): 1-23.
[^2]: See this very nice review D’Alessio, Luca, et al. "From quantum chaos and eigenstate thermalization to statistical mechanics and thermodynamics." Advances in Physics 65.3 (2016): 239-362. 
[^3]: see p2 Wigner, Eugene P. "Random matrices in physics." SIAM review 9.1 (1967): 1-23
[^4]: For example, see Goldford, Joshua E., et al. Science 361.6401 (2018): 469-474., Marsland III, Robert, Wenping Cui, and Pankaj Mehta. Scientific reports 10.1 (2020): 3308., Ho, Po-Yi, Benjamin H. Good, and Kerwyn Casey Huang. "Competition for fluctuating resources reproduces statistics of species abundance over time across wide-ranging microbiotas." Elife 11 (2022): e75168.
[^5]: This was a common perspective on generative protein models until the last five years. Recently, this narrative frame has retreated from popular conscience and been replaced by an almost exclusive focus on the machine learning architectures that enable one to learn such a distribution well.