---
title: "Nonequilibrium Boltzmann Distribution"
description: ""
summary: ""
date: 2024-12-04T18:59:06-06:00
lastmod: 2024-12-04T18:59:06-06:00
draft: false
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

Just as the equilibrium probability distribution can be expressed in terms of local energy \(U(x)\) via the Boltzmann law: $$p_{eq}(x) = e^{-\beta\; U(x)}/Z$$
So Rattling tell us that we can express non-equilibrium steady-states in terms of local Rattling value \(\mathcal{R}(x)\) as: $$p_{ss}(x) \approx e^{-\gamma\; \mathcal{R}(x)}/Z \tag{1}$$
This is a very powerful claim that has been sought by the nonequilibrium stat mech research community for decades, and so it comes at a price: the "\(\approx\)" in this expression is a poorly-controlled approximation. It generally works for "[[Typicality|typical]]" systems, but that notion so far lacks a formal definition. Some of the core questions in our research are thus understanding the assumptions and the practical generality of this approximation. #formal #general

The down-side of this is that currently, we don't have a clear formal method (beyond some rule-of-thumb intuitions) to a-priori decide how well expression (1) will hold for a given system. For example, many key results in nonequilibrium stat mech are derived from perturbative expansion for systems close to equilibrium – which is not the case here, and we have not identified any a-priori small parameter that yields (1) in the limit. 
The up-side is that this allows us to circumvent a core [[Landauer's blowtorch theorem|no-go theorem]] that held back progress in this area. In practice, we show that this expression holds for many systems arbitrarily far from equilibrium – regime where many other methods fail – thus allowing us to theoretically make predictions and engineer behaviors in these (see examples..). 
