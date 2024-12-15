---
title: Rattling Thermodynamics
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
---
Rattling gives us a "[[https://rattling.org/docs/background/neq-boltzmann/|Nonequilibrium Boltzmann Distribution]]" (a statement that must be carefully qualified and still needs further development and clarification, see link). This is something that has been sought by the nonequilibrium stat mech community for decades, and so if we suppose that we have this, it opens many possibilities. One natural next step is to try to translate the plethora of phenomena and results known from equilibrium thermodynamics to nonequilibrium systems, and verify them on experimental and numerical examples. 
Let's now go through a few research directions in more detail:

## Energy vs Rattling

Rattling plays the same role in non-equilibrium steady-state distributions (for [[https://rattling.org/docs/background/typicality|typical]] systems) as energy does in the Boltzmann distribution. This suggests comparing properties of Rattling $\mathcal{R}$ with those of energy, to see if $\mathcal{R}$ can be as powerful as energy for making predictions. One core question here is whether Rattling of a state is as easy to calculate as state energy. Another property of energy that is important is that it's locally conserved, and can flow among degrees of freedom (e.g., in the form of heat or work). Is there some equivalent of this for Rattling? While both of these questions seem implausible at first glance, some progress can, surprisingly, be made - see discussion on this [[https://rattling.org/docs/background/calc-rattling|here]] for some initial steps. 
## Entropy-energy tradeoff

In statistical mechanics, the tradeoff between energy and entropy is responsible for many of the most interesting predictions, such as phase transitions. This can directly translate to Rattling-entropy tradeoff, since when we coarse-grain the micro-state distribution $p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}$, we will naturally get $p_{ss}(X) \approx e^{-\gamma\; \mathcal{R}(X) + S(X)}$, where $S(X)$ is the entropy of the macro-state $X$. We explicitly show how this calculation can be carried out, and how it can predict the phase transition in the Vicsek model of flocking. 

## Random Energy Model

Also heat engines / Carnot cycle?

## Rattling-energy interactions



