---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

_Last Updated Nov. 2022_

# First-order Context-based Adaptation for Generalizing to New Dynamical Systems
---

![FOCA main](/images/FOCA.png "FOCA main")
![FOCA main2](http://junyoungpark.github.io/images/FOCA.png "FOCA main2")

http://junyoungpark.github.io/files/resume_junyoungpark.pdf

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

# Neuro CROSS exchange: Learning to CROSS exchange to solve realistic vehicle routing problems
---

[[Preprint]](https://arxiv.org/abs/2206.02771) CROSS exchange (CE), a meta-heuristic that solves various vehicle routing problems (VRPs), improves the solutions of
VRPs by swapping the sub-tours of the vehicles. Inspired by CE, we propose Neuro CE (NCE), a fundamental operator of
_learned_ meta-heuristic, to solve various min-max VRPs while overcoming the limitations of CE, i.e., the
expensive $\mathcal{O}(n^4)$ search cost. NCE employs graph neural network to predict the cost-decrements (i.e., results
of CE searches) and utilizes the predicted cost-decrements to guide the selection of sub-tours for swapping, while
reducing the search cost to $\mathcal{O}(n^2)$. As the learning objective of NCE is to predict the cost-decrement, the
training can be simply done in a supervised fashion, whose training samples can be easily collected. Despite the
simplicity of NCE, numerical results show that the NCE trained with min-max flexible multi-depot VRP (min-max FMDVRP)
outperforms the meta-heuristic baselines. More importantly, it significantly outperforms the neural baselines when
solving distinctive special cases of min-max FMDVRP (e.g., min-max MDVRP, min-max mTSP, min-max CVRP) without additional
training.