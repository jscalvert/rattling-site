---
title: Formalizing rattling
description: ""
summary: ""
date: 2024-12-04T18:59:06-06:00
lastmod: 2024-12-04T18:59:06-06:00
draft: false
weight: 30
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
author: Jacob Calvert
math: true
---

The upshot of [Landauer's blowtorch](/landauers-blowtorch) is that there can be no analogue of the Boltzmann distribution that applies to all nonequilibrium systems. As a consequence, it is not possible to analogously explain order in nonequilibrium systems. This suggests weakening the relation that the Boltzmann distribution constitutes, or narrowing the class of systems that must satisfy it. Rattling theory does both. We explain this point from a more mathematical perspective.

The following summarizes the key contribution of [Calvert and Randall, *PNAS* (2024)](https://www.pnas.org/doi/10.1073/pnas.2411731121). We can think of the Boltzmann distribution as an expression for the stationary distribution $p_{ss}$ of a finite, continuous-time Markov jump process.[^1] In terms of a function $U$ of the ingoing and outgoing rates of state $x$, this expression is:

$$ p_{ss} (x) \propto e^{-U(x)}. $$

We know that there is no "local" function $U$ that can satisfy this expression for all Markov jump processes. However, we can instead weaken the proportionality by observing that it is equivalent to perfect linear correlation between the logarithms of $p_{ss}$ and $-U$.

More precisely, let $X$ be a uniformly random state of the chain, and denote by $\rho$ the usual, linear correlation coefficient of $\log p_{ss} (X)$ and $-U(X)$.[^2] To be explicit,
$$
\rho = \frac{\mathrm{Cov}(\log p_{ss}(X),-U(X))}{\sqrt{\mathrm{Var}(\log p_{ss}(X))\mathrm{Var}(U(X))}}.
$$
The Boltzmann distribution is satisfied if and only if $\rho = 1$. A natural way to weaken the Boltzmann distribution is to allow $\rho$ to be less than $1$. We can then ask about the kinds of Markov chains that have a value of $\rho$ close to $1$, for a different local function of the rates. These chains are analogous to physical systems that satisfy an approximate analogue of the Boltzmann distribution, with a different local property of states in the place of energy. 

In fact, the natural choice of the function that plays a role analogous to energy is the logarithm of the sum of rates leaving each state, and, for this choice, we can derive a formula for $\rho$ in terms of properties of the Markov chain. To state this result requires some additional context, which a later entry will address. For now, we simply emphasize that generalizing the Boltzmann distribution means weakening the correlation that it normally entails, and finding a "local" function of the dynamics that produces strong correlation $\rho$ simultaneously for many systems. 





[^1]: Markov jump processes on finite state spaces are commonly used to model the dynamics underlying the steady-state distributions of nonequilibrium physical systems. For example, see [here](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.97.015002).

[^2]: It is not important that $X$ is uniformly random. Any distribution on $X$ for which the correlation coefficient is defined will work.
