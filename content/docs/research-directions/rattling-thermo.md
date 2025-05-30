---
title: Rattling thermodynamics
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
weight: 260
---
Rattling gives us a "[Nonequilibrium Boltzmann Distribution](https://rattling.org/docs/background/neq-boltzmann/)" (a statement that must be carefully qualified and still needs further development and clarification, see link). This is something that has been sought by the nonequilibrium stat mech community for decades, and so if we suppose that we have this, it opens many possibilities. One natural next step is to try to translate the plethora of phenomena and results known from equilibrium thermodynamics to nonequilibrium systems, and verify them on experimental and numerical examples. 
Let's now go through a few research directions in more detail:

## Energy vs Rattling

Rattling plays the same role in non-equilibrium steady-state distributions (for [typical](/docs/background/typicality) systems) as energy does in the Boltzmann distribution. This suggests comparing properties of Rattling $\mathcal{R}$ with those of energy, to see if $\mathcal{R}$ can be as powerful as energy in various contexts. See [here](/docs/research-directions/rattling-vs-energy) for details.

## Heat engines?

Another property of energy that is important is that it's locally conserved, and can flow among degrees of freedom (e.g., in the form of heat or work). Is there some equivalent of this for Rattling? This question is wide open at the moment. #open So much of our intuitions are based on energy that it's tough to translate to the very different context of Rattling - but if we suspend our habits and take a fresh perspective, we may be surprised. If this connection can be made, it would open up the territory of heat engines (e.g., Carnot cycle) for translation into Rattling context. 

## Entropy-energy tradeoff

In statistical mechanics, the tradeoff between energy and entropy is responsible for many of the most interesting predictions, such as phase transitions. This can directly translate to Rattling-entropy tradeoff, since when we coarse-grain the microstate distribution $p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}$, we will naturally get $p_{ss}(X) \approx e^{-\gamma\; \mathcal{R}(X) + S(X)}$, where $S(X)$ is the entropy of the macrostate $X$. We explicitly showed how this calculation can be carried out, and how it can predict the phase transition in the Vicsek model of flocking – [see here](/docs/examples/vicsek-model/). While it seemed to work in that example, the broader concept raises a [core question](/core-questions/#rattling-under-transformations) of how Rattling acts under coarse-graining (what is $\mathcal{R}(X)$ and how it relates to $\mathcal{R}(x)$ in general), whether there is a preferred level of granularity where Rattling is most accurate for steady-state prediction, and how to identify such granularity in new systems. #open

## Random Energy Model (REM)

This is a very simple and general model of equilibrium phase transitions in complex systems, like spin-glasses and proteins. It carries over nicely to the case of Rattling, showing us that we can similarly expect Rattling to cause such phase transitions in a wide variety of complex driven systems, and thus create strong fine-tuned selection of few least-Rattling states. See [here](/docs/examples/random-energy-model-rem/) for details.

## Rattling-energy interactions

The other interesting question is what happens in driven systems that have both, a strong energy landscape over their states, as well as a Rattling landscape. For strong driving, we might expect the driving to overwhelm any internal energies, making the energy-landscape hard to even define meaningfully (since energy is not conserved). However, in practice, the driving may not be strong enough to overwhelm all energetic effects, and we can somehow usefully define it.

In general, we don't expect a simple answer in these cases. Namely, we do NOT expect them to combine simply as $p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x) - \beta \; U(x)}/Z \tag{1}$. In our first paper on Rattling, we explored this question in a very simple 1D setting – and were able to verify some analytical predictions, see fig. 2 and 4 in [this paper](https://arxiv.org/abs/1707.03933). In more complex and general contexts, this question is still open. #open

