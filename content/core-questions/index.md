---
title: "Core Questions"
description: ""
summary: ""
date: 2024-12-06T15:49:26-06:00
lastmod: 2024-12-06T15:49:26-06:00
draft: false
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
## Typicality of rattling

**Rattling $\mathcal{R}(x)$ is a local property of a state $x$. How common are systems for which it strongly (anti)-correlates with the global steady-state distribution $p_{ss}(x)$?**

While we have many [examples](/docs/examples/summary/) of systems for which the rattling correlation holds in this sense, we still need to evaluate how commonly it holds among real-world systems.

There is also a mathematical version of this question, stemming from a [formula](/docs/background/formalizing-rattling/) for the rattling correlation in Markov jump processes, with recent [results](https://arxiv.org/abs/2505.01608).

## Strength of rattling fine-tuning

**In systems where rattling holds, can it produce a strongly concentrated $p_{ss}(x)$ distribution?**

To explain the remarkable degree of order found in nature, the fine-tuning due to rattling needs to be very strong, requiring $\mathcal{R}(x)$ to vary over several orders of magnitude. Is this possible and likely to happen in natural systems? 

See [examples](/docs/examples/summary/), specifically the discussion in [REM](/docs/examples/random-energy-model/).

## Environmental information encoding

**When can we say that the dynamical system is "learning" from its environment?**

Order in nature does not just mean selection of rare configurations—these configurations must also be recognizably "special." To talk about adaptation, this specialness must be in the way the configurations reflect the information in their external driving forces or environment.

See [this page](/docs/research-directions/learning-from-the-drive/) for some evidence and ideas on how to approach this.

## Rattling for transients

**Rattling is typically predictive of steady-state probabilities. Can it tell us anything about the transient dynamics?**

For questions of adaptation and origins of life, the key concern isn't whether life can be stable, but whether it can emerge on a reasonable timescale. So we must ask not only about the steady-state, but also about relaxation times and dynamics. 

One way to explore this question is to see if the theory of [rattling for Markov jump processes](/docs/background/formalizing-rattling/), which concerns the stationary distribution, also applies in some way to finite-time distributions.

This question is wide open, see [this page](/docs/research-directions/rattling-for-transients/) for what we know so far.

## Rattling workflow

**What is a principled and practical way to calculate rattling or estimate it from data?**

What can rattling do for you in your specific experiment or question?

See [here](/docs/background/how-to-use-rattling/) for details on experimental uses, and [here](/docs/research-directions/predicting-rattling/) for discussion on calculating or predicting it.


___
# More specific questions:

## Rattling under transformations

The extent to which rattling predicts a system's steady-state distribution depends on how the states are defined. If you transform the state space, say, by redefining your degrees of freedom or by coarse-graining, how does rattling change?

## Rattling under composition 

Rattling is a property of a state of a system. For systems that are groups of interacting elements (e.g., a flock of birds), a state might consist of the positions of all the elements (birds) in the group. Can we predict the rattling of such collective system state (flock) based on the rattling or dynamics of the individual elements (birds)? In other words, how can we go "one level down" in composite systems?

Note that rather than being just about coarse-graining (as in the question above), this is a question about "interaction rattling"—in parallel to "interaction energy" that we have in statistical mechanics. Perhaps even could there be some kind of renormalization group flow for rattling?

See [here](/docs/research-directions/predicting-rattling/#composability-of-rattling) for further discussion.

## Hierarchical self-organization

Most real-world examples of self-organization proceed in stages or hierarchically—e.g., first cells form, then multi-cellular organisms, then organism groups or societies, etc. While the rattling framework should be able to explain and predict such stepwise self-organization, we have yet to develop and study a clear example of this. Some interesting subtleties might arise here because intermediate stages present a scenario where some degrees of freedom are fine-tuned, while others remain "typical."

See [Examples](/docs/examples/summary/).

## *A priori* test of rattling

**How do we know for a given system if we should use rattling or not?**

Is it possible to use some simple measurements of the system to *a priori* know the success or failure of rattling to predict a system's steady-state distribution?

## Connections to other frameworks

**How does the rattling framework relate to other frameworks on nonequilibrium steady-states and self-organization?**

Especially, e.g., stochastic thermodynamics.
