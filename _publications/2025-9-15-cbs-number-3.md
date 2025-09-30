---
title: "Conflict-Based Search as a Protocol: A Multi-Agent Motion Planning Protocol for Heterogeneous Agents, Solvers, and Independent Tasks"
collection: publications
category: manuscripts
permalink: /publication/2025-9-15-cbs-number-2
date: 2025-09-15
venue: 'under review'
header:
  teaser: cbs_teaser.png
paperurl: 'coming soon'
website: "https://rishi-v.github.io/CBS-Protocol/"
excerpt: "co-second author, alphabetical order"
authors: "Rishi Veerapaneni, Alvin Tang<sup>*</sup>, Haodong He<sup>*</sup>, Sophia Zhao<sup>*</sup>, Viraj Shah<sup>*</sup>, Yidai Cen<sup>*</sup>, **Ziteng Ji**<sup>*</sup>, Gabriel Olin<sup>†</sup>, Jon Arrizabalaga<sup>†</sup>, Yorai Shaoul<sup>†</sup>, Jiaoyang Li, Maxim Likhachev"
---

Rishi Veerapaneni, Alvin Tang<sup>*</sup>, Haodong He<sup>*</sup>, Sophia Zhao<sup>*</sup>, Viraj Shah<sup>*</sup>, Yidai Cen<sup>*</sup>, **Ziteng Ji**<sup>*</sup>, Gabriel Olin<sup>†</sup>, Jon Arrizabalaga<sup>†</sup>, Yorai Shaoul<sup>†</sup>, Jiaoyang Li, Maxim Likhachev

<sup>*</sup> (Equal contribution)
<sup>†</sup> (Equal contribution)

Imagine the future construction site, hospital, office, or even sophisticated household with dozens of robots bought from different manufacturers. How can we enable these different systems to effectively move in a shared environment, given that each robot may have its own independent motion planning system?
This work shows how we can get efficient collision-free movements between algorithmically heterogeneous agents by using Conflict-Based Search (Sharon et al. 2015) as a protocol.
At its core, the CBS Protocol requires one specific single-agent motion planning API; finding a collision-free path that satisfies certain space-time constraints. Given such an API, CBS uses a central planner to find collision-free paths - independent of how the API is implemented.
We show how this protocol enables multi-agent motion planning for a heterogeneous team of agents completing independent tasks with a variety of single-agent planners including: Heuristic Search (e.g., A*), Sampling Based Search (e.g., RRT), Optimization (e.g., Direct Collocation), Diffusion, and Reinforcement Learning.
