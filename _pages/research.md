---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

_Last Updated Nov. 2022_

# First-order Context-based Adaptation for Generalizing to New Dynamical Systems

![FOCA main](/images/research/FOCA.png)

[[Preprint]](https://arxiv.org/abs/2206.00694) In this paper, we propose FOCA (First-Order Context-based Adaptation),
a learning framework to model sets of systems governed by common but unknown laws that differentiate themselves by their
context.
Inspired by classical modeling-and-identification approaches, FOCA learns to represent the common law through shared
parameters and relies on online optimization to compute system-specific context.
Due to the online optimization-based context inference,
the training of FOCA involves a bi-level optimization problem.
To train FOCA efficiently, we utilize an exponential moving average (EMA)-based method that
allows for fast training using only first-order derivatives.
We test FOCA on polynomial regression and time-series prediction tasks composed of
three ODEs and one PDE, empirically finding it outperforms baselines.

