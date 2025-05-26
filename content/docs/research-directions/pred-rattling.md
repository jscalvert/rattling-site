---
title: Predicting Rattling
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
weight: 210
---
\[For broader context, see [Rattling Thermodynamics](https://rattling.org/docs/background/rattling-thermo/)]
One limitation of the Rattling framework $p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}/Z \tag{1}$  is that for arbitrary far-from-equilibrium nonlinear dynamical systems, it is difficult to analytically estimate Rattling of any given state $\mathcal{R}(x)$. So we often need to explicitly measure $\mathcal{R}(x)$. This still allows us to predict global steady-state in terms of only local measurements of Rattling, and so is already practically useful, but the cases where we can predict $\mathcal{R}(x)$ analytically allow for much more prediction and control. 

## Composability of energy

This can be compared to the equilibrium counter-part, the Boltzmann distribution $p_{eq}(x) = e^{-\gamma\; U(x)}/Z$ , where the state energy $U(x)$ can often be calculated analytically even for very complex equilibrium systems. Now notice that there is no fundamental sense in which state energy should be any more "natural" or "simple" to deal with than Rattling – the latter is in fact easier to access experimentally using only a single local measurement (by just checking the state exit rate). The main reason why energy $U(x)$ is so useful in equilibrium systems is because it is conserved (which leads to the Boltzmann distribution), and *composable* (which means that the energy of any complex system state is just the sum of all constituent subsystem energies and interaction energies).

So if there was a way to calculate the Rattling of a complex composite system from knowing something about the Rattling of the component dynamics and their interactions, then our framework would be comparable in predictive power to the equilibrium stat mech. 

## Composability of Rattling?

#### Independent systems
While this is probably too much to ask in the general case, some progress can likely be made. To begin, we notice that for non-interacting subsystems $A$ and $B$, steady-state probability distribution factors, and so Rattling is indeed composable:  $p_{ss}(x_{AB}) = p_{ss}(x_A)\; p_{ss}(x_B) \approx e^{-\gamma\; \left(\mathcal{R}(x_A)+\mathcal{R}(x_B)\right)}/Z$. We can also verify this from directly calculating Rattling of the composite system: remembering that for continuous systems $\mathcal{R}(x_{AB}) = \frac{1}{2} \log \det \mathcal{C}(x_{AB})$, in terms of the covariance matrix $\mathcal{C}$, which will be block-diagonal for a system composed of two independent subsystems, giving $\det \mathcal{C}_{AB} = \det \mathcal{C}_A\,\det \mathcal{C}_B$, thus consistently recovering $\mathcal{R}(x_{AB}) = \mathcal{R}(x_{A}) + \mathcal{R}(x_{B})$.

This suggest one possible research direction:
* Perturbatively turn on weak interactions, and see how this affects the composite Rattling values, look for general principles that may extend beyond the perturbative regime. This is similar to the treatment of weakly-coupled field theories, which may, in fact, be a good example to study this on (see Anharmonic Net example [FIX link]). 

#### Stochastic systems
Another example where we can use composition is if one of the systems is so chaotic that it can be estimated as state-independent noise: $\mathcal{R}_{B} = const$, and so that interactions just serve to "raise the temperature" of the composite. This suggests another research direction:
* For any interaction strengths, look for ways to decompose the composite system Rattling in terms of subsystem Rattlings and some additional "interaction contribution" – which we can always define as $\mathcal{R}_{int} \equiv \mathcal{R}_{AB}-\mathcal{R}_A-\mathcal{R}_B$. The question is then whether this $\mathcal{R}_{int}$ has some nice properties and may be analytically predicted in some cases. One hypothesis would be that it may be estimated in terms of the relationship between the symmetries in the driving force and the symmetries of the composite system state $AB$ – so in the above case of "$B$ as noise," there are no compatible symmetries, and so $\mathcal{R}_{int}=0$.

#### Composing over driving force components
Yet another interesting approach comes from composing Rattling not out of its subsystems, as is done with energy, but rather out of the different components of its driving force. This was successfully demonstrated in our Science paper, fig 2 and 3, [FIX link] where it allowed us to analytically predict and engineer the steady-state behaviors of a robot swarm. 

#### "Analytic continuation" of Rattling landscape
More generally, this suggests another route to analytically predicting Rattling – by measuring it for some parameter regime of a system, and then using that to predict how the Rattling landscape $\mathcal{R}(x)$ will evolve as we adjust the parameters. Though perhaps this path seems more system specific, and less likely to yield a general "cookbook."