---
title: Random Energy Model (REM)
description: ""
summary: ""
date: 2024-12-04T18:53:05-06:00
lastmod: 2024-12-04T18:53:05-06:00
draft: false
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
author: Pavel Chvykov
---
One of the simplest, and also most general, models of equilibrium phase transition is the [REM](https://en.wikipedia.org/wiki/Random_energy_model). Here, we consider the case where the energies of the accessible system states are normally distributed $\{U(x)\} \sim \mathcal{N}(0, \sigma)$. This is motivated by the central limit theorem, and applies in cases where the state energy is a sum of many interaction energies that are so messy as to be essentially random – as may be the case for a spin-glass or a folded protein. This model is a prime example of using the assumption of [typicality](https://rattling.org/docs/background/typicality) . 

This model can then be shown to exhibit a phase transition. Since at equilibrium, $p_{eq}(x) \propto e^{-\beta\, U(x)}$, we have a log-normal distribution of state probabilities, whose tale thickness is controlled by the inverse temperature $\beta$ ($\sigma$ above is considered a system-specific constant). When the tale becomes especially thick (at high $\beta$ = low temperature), the probability distribution becomes dominated by the few states deep in the tale of low $U(x)$. This leads to a low-entropy fine-tuned selection of microstates reminiscent of the "frozen" or "solid" phase. 

## Random Rattling Model

For Rattling, we might similarly expect $\{\mathcal{R}(x)\} \sim \mathcal{N}(0, \sigma)$ – but this needs to be checked more carefully [OPEN]. While energy of a state is *compositional* – it is the sum of all the subsystem interaction energies – the Rattling of a state does not always have this property (though sometimes it does – see [here](https://rattling.org/docs/background/calc-rattling)). Alternatively, we can remember its definition $\mathcal{R} = \frac{1}{2} \log \det \mathcal{C}$ in terms of the correlation matrix $\mathcal{C}_{ij} = \left<\dot{x}_i, \dot{x}_j\right>$. Here, looking for the *typical* distribution of Rattling in a complex system, puts us in the territory of random matrix theory: if we can assume that the correlations are so messy as to be essentially random, then we are looking for log det of a random symmetric positive semi-definite matrix. [This paper](https://arxiv.org/pdf/1309.0482) showed that this may actually be Gaussian distributed – taking us back to where we started. In general, however, this will depend on the specific random matrix ensemble, and so we need to consider carefully our specific case. 

Empirically, however, we see that Rattling does tend to be normally distributed for many complex dynamical systems. This means that the REM results carry over directly, predicting two possible phases for dynamical system steady-states: when the variance of Rattling values across system states is high, we'll expect probability to concentrate strongly in the few least-Rattling states in the tail of the distribution. Besides giving a nice example of a Rattling-driven phase transition, this also addresses one of the core questions of this research [FIX link] – whether Rattling effects are typically strong enough to create strong fine-tuning. 