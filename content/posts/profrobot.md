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

<div>
<button style="background-color: #007bff; color: white; border: none; padding: 10px 20px; border-radius: 5px; margin-right: 10px;" onclick="window.location.href='https://arxiv.org/abs/2503.11269'"><strong>Paper</strong></button>
<button style="background-color: #28a745; color: white; border: none; padding: 10px 20px; border-radius: 5px; margin-right: 10px;" onclick="window.location.href='https://github.com/qrcat/prof.robot'"><strong>Code</strong></button>
<button style="background-color: #ffc107; color: white; border: none; padding: 10px 20px; border-radius: 5px; margin-right: 10px;" onclick="window.location.href='/prof-robot'"><strong>Project</strong></button>
</div>

