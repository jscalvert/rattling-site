---
title: Nonequilibrium Boltzmann distribution
description: ""
summary: ""
date: 2024-12-04T18:59:06-06:00
lastmod: 2024-12-04T18:59:06-06:00
draft: false
weight: 20
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
author: Pavel Chvykov
math: true
---

There can be no analogue of the Boltzmann distribution that applies to all nonequilibrium systems. Consequently, there can be no analogous explanation of order in nonequilibrium systems. Progress therefore requires weakening the relation that the Boltzmann distribution constitutes, or narrowing the class of systems that must satisfy it. Rattling theory does both. We explain this point from two perspectives. The first is physical; the [second](#a-mathematicians-perspective) is more mathematical.

### A physicist's perspective

Just as the equilibrium probability distribution can be expressed in terms of local energy $U(x)$ via the Boltzmann law: $$p_{eq}(x) = e^{-\beta\; U(x)}/Z$$
So Rattling tell us that we can express non-equilibrium steady-states in terms of local Rattling value $\mathcal{R}(x)$ as: $$p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}/Z \tag{1}$$
This is a very powerful claim that has been sought by the nonequilibrium stat mech research community for decades, and so it comes at a price: the "$\approx$" in this expression is a poorly-controlled approximation. It generally works for "[typical](https://rattling.org/docs/background/typicality/)" systems, but that notion so far lacks a formal definition. Some of the core questions in our research are thus understanding the assumptions and the practical generality of this approximation. #formal #general

The down-side of this is that currently, we don't have a clear formal method (beyond some rule-of-thumb intuitions) to a-priori decide how well expression (1) will hold for a given system. For example, many key results in nonequilibrium stat mech are derived from perturbative expansion for systems close to equilibrium – which is not the case here, and we have not identified any a-priori small parameter that yields (1) in the limit. 
The up-side is that this allows us to circumvent a core [no-go theorem](https://rattling.org/docs/background/landauers-blowtorch/) that held back progress in this area. In practice, we show that this expression holds for many systems arbitrarily far from equilibrium – regime where many other methods fail – thus allowing us to theoretically make predictions and engineer behaviors in these (see examples..). 

### A mathematician's perspective

The following summarizes the key contribution of [Calvert and Randall, *PNAS* (2024)](https://www.pnas.org/doi/10.1073/pnas.2411731121). As in the previous entry, we can think of the Boltzmann distribution as an expression for the stationary distribution $\pi$ of a finite, continuous-time Markov chain. In terms of a function $E$ of the ingoing and outgoing rates of state $x$, this expression is:

$$ \pi (x) \propto e^{-E(x)}. $$

We know that there is no "local" function $E$ that can satisfy this expression for all Markov chains. However, we can instead weaken the proportionality by observing that it is equivalent to perfect linear correlation between the logarithms of $\pi$ and $-E$.

More precisely, let $X$ be a uniformly random state of the chain, and denote by $\rho$ the usual, linear correlation coefficient of $\log \pi (X)$ and $-E(X)$.[^1] To be explicit,
$$
\rho = \frac{\mathrm{Cov}(\log\pi(X),-E(X))}{\sqrt{\mathrm{Var}(\log\pi(X))\mathrm{Var}(E(X))}}.
$$
The Boltzmann distribution is satisfied if and only if $\rho = 1$. A natural way to weaken the Boltzmann distribution is to allow $\rho$ to be less than $1$. We can then ask about the kinds of Markov chains that have a value of $\rho$ close to $1$, for a different local function of the rates. These chains are analogous to physical systems that satisfy an approximate analogue of the Boltzmann distribution, with a different local property of states in the place of energy. 

In fact, there is a natural choice of the function that plays a role analogous to energy and, for this choice, we can derive a formula for $\rho$ in terms of properties of the Markov chain. To state this result requires some additional context, which a later entry will address.





 

[^1]: It is not important that $X$ is uniformly random. Any distribution on $X$ for which the correlation coefficient is defined will work.
