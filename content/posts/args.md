---
title: 'ARGS: Auto-Regressive Gaussian Splatting via Parallel Progressive Next-Scale Prediction'
date: '2026-07-04T22:39:50+08:00'
tags: ["AIGC", "3D Generation"]
author: ["Quanyuan Ruan", "Kewei Shi", "Jiabao Lei", "Xifeng Gao", "Xiaoguang Han"]
draft: false
description: "CVPR2026 Findings"
# cover:
#     image: "<image path/url>" # image path/url
#     alt: "<alt text>" # alt text
#     caption: "<text>" # display caption under cover
#     relative: false # when using page bundles set this to true
#     hidden: true # only hide on current single page
---

Auto-regressive frameworks for next-scale prediction of 2D images have demonstrated strong potential for producing diverse and sophisticated content by progressively refining a coarse input. However, extending this paradigm to 3D object generation remains largely unexplored. In this paper, we introduce auto-regressive Gaussian splatting (ARGS), a framework for making next-scale predictions in parallel for generation according to levels of detail. We propose a Gaussian simplification strategy and reverse the simplification to guide next-scale generation. Benefiting from the use of hierarchical trees, the generation process requires only O(log n) steps, where n is the number of points. Furthermore, we propose a tree-based transformer to predict the tree structure auto-regressively, allowing leaf nodes to attend to their internal ancestors to enhance structural consistency. Extensive experiments demonstrate that our approach effectively generates multi-scale Gaussian representations with controllable levels of detail, visual fidelity, and a manageable time consumption budget.

<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=116913757751148&bvid=BV1sXNU6fEFa&cid=39922175332&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

[Paper](https://openaccess.thecvf.com/content/CVPR2026F/html/Ruan_ARGS_Auto-Regressive_Gaussian_Splatting_via_Parallel_Progressive_Next-Scale_Prediction_CVPRF_2026_paper.html)|[Code](https://github.com/qrcat/ARGS_official)|[Output](https://drive.google.com/drive/folders/1dJfWJw3uUad9FubzWSbI9ur1uDkdVwxk?usp=sharing)

```bib
@InProceedings{Ruan_2026_CVPR,
    author    = {Ruan, Quanyuan and Shi, Kewei and Lei, Jiabao and Gao, Xifeng and Han, Xiaoguang},
    title     = {ARGS: Auto-Regressive Gaussian Splatting via Parallel Progressive Next-Scale Prediction},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Findings},
    month     = {June},
    year      = {2026},
    pages     = {8439-8448}
}
```