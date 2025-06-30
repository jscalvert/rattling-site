---
title: List of examples
description: ""
summary: ""
date: 2024-12-04T18:53:05-06:00
lastmod: 2024-12-04T18:53:05-06:00
draft: false
weight: 110
seo:
  title: ""
  description: ""
  canonical: ""
  noindex: false
---
Here are several entries from an ever-growing list of examples, which we will add to the website over time:

- **Dynamics of spin systems.** For example, the [random energy model (REM)](http://rattling.org/docs/examples/random-energy-model/) is a random probability distribution on configurations of "spins" that take values of $\pm 1$. The probability distribution is the Boltzmann distribution corresponding to a random energy landscape. One way to sample configurations from this distribution is to run a Markov chain whose stationary distribution is the appropriate Boltzmann distribution. Rattling predicts the stationary distribution of this Markov chain well. The same is true of dynamics of the Sherrington–Kirkpatrick model in various parameter regimes.
- **Models of animal collective behavior.** Rattling predicts the steady-state distributions of many models of animal collective behavior for relevant ranges of model parameters. Examples include the [Föllmer–Kirman](https://academic.oup.com/qje/article-abstract/108/1/137/1898484) model of binary decision-making by ant colonies and the [Beekman–Ratnieks–Sumpter](https://www.pnas.org/doi/10.1073/pnas.161285298) model of trail formation.  Additional examples include the [Jhawar et al.](https://www.nature.com/articles/s41567-020-0787-y) model of noise-induced schooling in fish and the [Amé et al.](https://www.sciencedirect.com/science/article/pii/S0003347204002210?casa_token=ePxwazgaDeUAAAAA:xiitV_jTfckSpJK-oPIIXbQVh7vzcVCrSXRRaOhNAOBUAQuM_7UcDpHKTLbu2IQOkaP6H1jC9f0) model of shelter selection by cockroaches. There are many more!
- **Models of ecological succession.** Ecological succession entails changes in the composition of an ecosystem over time. Rattling can also predict the steady-state distribution of these compositions. Examples include succession in communities of microbes, mites, and subtidal and forest ecologies.
- **Various random walk models.** Rattling can be studied in large classes of random Markov chains by putting various distributions (e.g., power law) on the transition rates, with various underlying connectivities (e.g., densely connected or sparsely connected).
- **[Random chemical reaction system](http://rattling.org/docs/examples/random-chemistry/).** A model of a chemical reaction system in which a fixed number of species react with random rate constants. The maximum molecularity of the reactions is also fixed.