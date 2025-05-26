---
title: Learning from the drive
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
weight: 220
---
What makes Rattling theory especially interesting is that while it starts as a simple claim about system dynamics, it leads to a claim about information content of selected system configurations and learning from the drive. 

The basic idea is:
* Rattling hypothesis is "survival of the stablest" - you end up in places that you don't leave
* If your environment is violent and complex, being stable in it requires learning to predict it
* So does this give us a general theory of abiotic adaptation and learning?

Roughly speaking, this seems plausible, but some work is still needed to formalize and clarify the exact claims and their proofs. 

## Smarticles 
<img src="drive_learn.png" alt="drawing" style="max-width: 600px; width: 100%; height: auto;"/>
Steady-state distributions encode drive properties. (A) shows 4 distinct arm-motion patterns, in order of increasing predictable information content, from fully random to an intricate periodic form. (B) shows their corresponding steady-state distributions (note different orientation of the 3D axes compared to Fig. 2 and fig. S5). Reflecting drive properties, these get concentrated into smaller fraction of configuration space for more intricate drives. (C) quantifies this effect by showing distribution entropies. Applying each of the 4 drives to the uniform initial distribution (grey star), we can see how drive information gets gradually imprinted on it, causing the low-entropy fine-tuning in the steady-state, with more intricate drives causing more fine-tuning. Finally, to quantify the specificity of each distribution to its drive, we calculate “distances” between pairs of distributions as relative entropies DKL. We then use these in (D) to visualize the path that /2 distributions take as they evolve from uniform initial conditions under the influence of their respective drive. Starting from the same point, we can see precisely how their shapes diverge over time.

Add fig from Science SI, and discuss Bayes encoding (link paper)