---
title: Explaining order
description: 
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 10
toc: true
seo:
  title: ""
  description: ""
  canonical: ""
  robots: ""
math: true
---

Systems across physical scales and scientific domains exhibit order. Proteins fold, cells become tissues, and army ants form nests of their living bodies.[^1] To us, a system exhibits order when it spends a disproportionate fraction of time in relatively few of the "states" available to it.[^2] In many instances, this kind of temporal order goes hand in hand with spatial order, like a crystalline solid. Explaining how order arises is a fundamental scientific challenge.

### The Boltzmann distribution

For systems in thermal equilibrium, there is a powerful explanation of order. A property of each state, called energy, determines the long-run fraction of time that the system spends in it. States with lower energy are favored to an extent determined by temperature, which is quantified by the Boltzmann distribution, the cornerstone of statistical mechanics:

$$ P(x) = \frac{1}{Z} e^{-E(x)/T}. $$

In this expression, $P(x)$ denotes the long-run fraction of time that the system spends in state $x$, which can be thought of as the probability that you would observe the system in $x$. The energy of $x$ is denoted by $E(x)$, $T$ is the temperature, and $Z$ is the quantity that ensures $P$ sums to one.

### Local explains global

The energy of a state is "local" in the sense that it can be determined without reference to any other state. For example, if $x$ represents a protein conformation, then $E(x)$ can be calculated from the positions of the molecules that it comprises. It isn't important to know how one conformation becomes another, or how long it takes to do so. In contrast, the long-run fraction of time spent in each state is a "global" property of a system. Determining $P$ generally requires observing the system for a long time, as it transitions through many other states. The Boltzmann distribution is remarkable because it explains a global thing in terms of a local thing.

### The problem

Unfortunately, the Boltzmann distribution—and the explanation of order it provides—applies only to systems in thermal equilibrium. In particular, it does not apply to the many spectacular forms of order that living and driven systems exhibit. In fact, there can be no analogous explanation of order that applies to all nonequilibirum systems. This is the upshot of "[Landauer's blowtorch](/docs/background/landauers-blowtorch)."



[^1]: This kind of nest is called a bivouac.
[^2]: We mean the long-run fraction of time spent in a state. Implicit in our discussion is the assumption that the system reaches a steady or stationary state.
