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
Systems across physical scales and scientific domains exhibit order. Proteins fold, cells become tissues, and army ants form nests of their living bodies.[^1] However, to study order in nature, we must be careful in defining it: On the one hand, it refers to *"[concentration](/core-questions/#strength-of-rattling-fine-tuning)"* – the system spending most of its time in a very small fraction of all possible configurations or states. However, many natural systems that are trapped in some configuration can still be "disordered." So a second requirement must be introduced – that these few selected configurations are also recognizably *"[special](/core-questions/#environmental-information-encoding)."* This can come in the form of spatial order – such as with pattern formation like crystals or zebra stripes, or in the form of function – such as with living organisms. While equilibrium thermodynamics helps us understand a special case of order – self-assembly – the case of order, and especially functional order, in presence of energy sources remains largely open. 

### The Boltzmann distribution

For systems in thermal equilibrium, there is a powerful explanation of order – specifically of self-assembly. A property of each state, called energy, determines the long-run fraction of time that the system spends in it. States with lower energy are favored to an extent determined by temperature, which is quantified by the Boltzmann distribution, the cornerstone of statistical mechanics:

$$ P(x) = \frac{1}{Z}\; e^{-U(x)/T}. $$

In this expression, $P(x)$ denotes the long-run (steady-state) probability that the system is found in state $x$. For ergodic systems, this is also the long-run fraction of time that the system spends in state $x$. The energy of $x$ is denoted by $U(x)$, $T$ is the temperature, and $Z$ is the normalization that ensures $P$ sums to one.

### Local explains global

The energy of a state is "local" in the sense that it can be determined without reference to any other state. For example, if $x$ represents a protein conformation, then $U(x)$ can be calculated from the positions of the molecules that it comprises. It isn't important to know how one conformation becomes another, or how long it takes to do so. In contrast, the long-run fraction of time spent in each state is a "global" property of a system. Determining $P(x)$ generally requires observing the system for a long time, as it transitions through many other states. The Boltzmann distribution is remarkable because it explains a global thing $P(x)$ in terms of a local thing $U(x)$.

### The problem

Unfortunately, the Boltzmann distribution—and the explanation of order it provides—applies only to systems in thermal equilibrium. In particular, it does not apply to the many spectacular forms of order that living and driven systems exhibit. In fact, there can be no analogous explanation of order that applies to all nonequilibirum systems. This is the upshot of "[Landauer's blowtorch theorem](/docs/background/landauers-blowtorch)." Rattling theory circumvents this no-go theorem by weakening two its conditions, and thus makes possible a sort of [nonequilibrium Boltzmann distribution](/docs/background/nonequilibrium-boltzmann-distribution/), which we can then use to explain order – both the "concentration," and the "functional specialness" of the selected states.



[^1]: This kind of nest is called a bivouac.
[^2]: We mean the long-run fraction of time spent in a state. Implicit in our discussion is the assumption that the system reaches a steady or stationary state.
