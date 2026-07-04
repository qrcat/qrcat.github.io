---
title: 'DreamUV: Unwrap Artist-like UV by End-to-End Flow Matching'
date: '2026-07-04T22:46:03+08:00'
tags: ["AIGC", "CG"]
author: ["Quanyuan Ruan", "Jiabao Lei", "Xingyi Du", "Xifeng Gao"]
draft: false
description: "arXiv preprint"
# cover:
#     image: "<image path/url>" # image path/url
#     alt: "<alt text>" # alt text
#     caption: "<text>" # display caption under cover
#     relative: false # when using page bundles set this to true
#     hidden: true # only hide on current single page
---

UV parameterization is a fundamental step in 3D content creation, yet producing production-ready UV layouts remains challenging due to the gap between geometric distortion objectives and the stylistic preferences of professional artists. While classical methods optimize handcrafted energy functions, artist-authored UVs exhibit structural patterns such as straightened seams, axis-aligned islands, and flexible interior deformation, properties that are difficult to explicitly formulate. In this work, we present DreamUV, an end-to-end learning framework that formulates UV unwrapping as a generative Flow Matching problem. Rather than predicting a single optimal parameterization, DreamUV learns a mesh-conditioned transport process that maps noise samples to a distribution of artist-like UV layouts. To reflect real-world authoring practices, we introduce a boundary-aware training strategy that prioritizes seam geometry, and a Model-in-the-Loop Finetuning(MITL) scheme that explicitly accounts for discretization errors during sampling and stabilizes transport dynamics under heterogeneous supervision. We evaluate DreamUV on a large-scale dataset of professionally authored UV layouts. Experiments demonstrate that our method produces significantly straighter boundaries and tighter axis-aligned islands than both classical and learning-based baselines, while maintaining competitive distortion metrics. Qualitative results and a user study with professional artists further confirm that DreamUV generates UV layouts that are not only valid, but aligned with practical production requirements.

[Paper](https://arxiv.org/abs/2606.22445)

```bib
@online{ruan2026dreamuv,
  author        = {Quanyuan Ruan and Jiabao Lei and Xingyi Du and Xifeng Gao},
  title         = {DreamUV: Unwrap Artist-like UV by End-to-End Flow Matching},
  year          = {2026},
  eprint        = {2606.22445},
  archivePrefix = {arXiv},
  primaryClass  = {cs.CV},
  url           = {https://arxiv.org/abs/2606.22445},
}
```