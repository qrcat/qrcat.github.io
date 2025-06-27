---
title: 'Prof. Robot: Differentiable Robot Rendering Without Static and Self-Collisions'
date: '2025-03-14T19:45:55+08:00'
tags: ["Robotics", "Differentiable Rendering"]
author: ["Quanyuan Ruan", "Jiabao Lei", "Wenhao Yuan", "Yanglin Zhang", "Dekun Lu", "Guiliang Liu", "Kui Jia"]
draft: false
description: "CVPR2025"
cover:
    image: "/prof-robot//static/images/teaser.png" # image path/url
    alt: "By learning and integrating a gradient-consistent pose classifier into a differentiable rendering pipeline, the generated pose trajectories are free from physical collisions. The objective is to penalize high collision probabilities during optimization." # alt text
    caption: "Prof.Robot improves upon Dr.Robot by additionally enabling differentiable avoidance of static and self-collisions." # display caption under cover
---

Differentiable rendering has gained significant attention in the field of robotics, with differentiable robot rendering emerging as an effective paradigm for learning robotic actions from image-space supervision. However, the lack of physical world perception in this approach may lead to potential collisions during action optimization. In this work, we introduce a novel improvement on previous efforts by incorporating physical awareness of collisions through the learning of a neural robotic collision classifier. This enables the optimization of actions that avoid collisions with static, non-interactable environments as well as the robot itself. To facilitate effective gradient optimization with the classifier, we identify the underlying issue and propose leveraging Eikonal regularization to ensure consistent gradients for optimization. Our solution can be seamlessly integrated into existing differentiable robot rendering frameworks, utilizing gradients for optimization and providing a foundation for future applications of differentiable rendering in robotics with improved reliability of interactions with the physical world. Both qualitative and quantitative experiments demonstrate the necessity and effectiveness of our method compared to previous solutions.

[Paper](https://openaccess.thecvf.com/content/CVPR2025/html/Ruan_Prof._Robot_Differentiable_Robot_Rendering_Without_Static_and_Self-Collisions_CVPR_2025_paper.html) | [Code](https://github.com/qrcat/prof.robot) | [Project](/prof-robot)

```bib
@InProceedings{Ruan_2025_CVPR,
    author    = {Ruan, Quanyuan and Lei, Jiabao and Yuan, Wenhao and Zhang, Yanglin and Lu, Dekun and Liu, Guiliang and Jia, Kui},
    title     = {Prof. Robot: Differentiable Robot Rendering Without Static and Self-Collisions},
    booktitle = {Proceedings of the Computer Vision and Pattern Recognition Conference (CVPR)},
    month     = {June},
    year      = {2025},
    pages     = {22562-22572}
}
```
