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

*Rattling $\mathcal{R}(x)$ is a local property of a state $x$ – how common are systems for which it is strongly correlated with its probability $p_{ss}(x)$ in the global steady-state distribution?*

While we have many [examples](/docs/examples/) of classes of systems for which rattling hypothesis holds in this sense, we still need a better evaluation of how common this is among real-world systems.

(see here[LINK Jacob's result] for our best understanding of this so far)

## Strength of rattling fine-tuning

*In systems where rattling holds, can it produce a strongly concentrated $p_{ss}(x)$ distribution?*

To explain the remarkable degree of organization and order found in nature, the fine-tuning due to Rattling needs to be very strong, requiring $\mathcal{R}(x)$ to vary over several orders of magnitude. Is this possible and likely to happen in natural systems? 

(see [examples](https://rattling.org/docs/examples/), and specifically the discussion in [REM](/docs/examples/random-energy-model/))

## Environmental information encoding

*When can we say that the dynamical system is "learning" from its environment?*

"Order" in nature does not just mean selection of rare configurations – these configurations must also be recognizably "special." To talk about adaptation, this "specialness" must be in the way the configurations reflect the information in their external driving forces or environment. 

(see this discussion[LINK learning from the drive] for some evidence and ideas on how to approach this)

## Rattling for transients

*Rattling is typically predictive of steady-state probabilities. Can it tell us anything about the transient dynamics?*

For questions of adaptation and origins of life, the key concern isn't whether life can be stable, but whether it can emerge on a reasonably fast time-scale. So we must ask not only about the steady-state, but also about relaxation times and dynamics. 

[I like yours, but can you tie it in with the above, and also make it a bit less technical? Also I think can drop first 2 sentences as they are repeats]
Rattling relates a local property of a state to its weight in the global steady-state distribution. The Markov chain theory of rattling shows that this local property suffices to predict the global weight of a state when the local part varies enough over the states of the system. Does this view of rattling hold even when the global steady-state distribution is replaced by a finite-time distribution?

(this is a wide open question, see this discussion[LINK transient] for what we know so far)

## Rattling workflow

*What is a principled and practical way to calculate Rattling or estimate it from data?*
What can Rattling do for you in your specific experiment or question, and how to work with it?

(see [here](/docs/background/how-to-use-rattling/) for details on experimental uses, and [here](/docs/research-directions/predicting-rattling/) for discussion on calculating / predicting it)


___
# More specific questions:

## Rattling under transformations

The extent to which rattling predicts a system's steady-state distribution depends on how the states are defined. If you transform the state space, say, by redefining your degrees of freedom or by coarse-graining, how does rattling change?

## Rattling under composition 

Rattling is a property of a state of a system. For systems that are groups of interacting elements (e.g., a flock of birds), a state might consist of the positions of all the elements (birds) in the group. Can we predict the rattling of such collective system state (flock) based on the rattling or dynamics of the individual elements (birds)? In other words, how can we go "one level down" in composite systems? 
Note that rather than being just about coarse-graining (as in the question above), this is a question about "interaction Rattling" – in parallel to "interaction energy" that we have in stat. mech. Perhaps even could there be some "Renormalization Group" flow for Rattling?

(see [here](/docs/research-directions/predicting-rattling/#composability-of-rattling) for discussion, and the [anharmonic net] example)

## Hierarchical self-organization

Most real-world examples of self-organization proceed in stages or hierarchically – e.g., first cells form, then multi-cellular organisms, then organism groups or societies, etc. While the rattling framework should be able to explain and predict such step-wise self-organization, we have yet to develop and study a clear example of this. Some interesting subtleties might arise here because intermediate stages present a scenario where some degrees of freedom are fine-tuned, while others remain "typical."

(see [Vicsek model](/docs/examples/vicsek-model/), [Kicked Harmonic Net] and [kicked lattice] examples)

## *A priori* test of rattling

*How do we know for a given system if we should use Rattling or not?*
Is it possible to use some simple measurements of the system to *a priori* know the success or failure of rattling to predict a system's steady-state distribution?

## Connections to other frameworks

*How does the Rattling framework relate to other frameworks on non-equilibrium steady-states and self-organization?*
