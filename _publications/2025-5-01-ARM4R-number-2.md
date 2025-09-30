---
title: "Pre-training Auto-regressive Robotic Models with 4D Representations"
collection: publications
category: manuscripts
permalink: /publication/2025-5-01-ARM4R-number-2
excerpt: 'ARM4R, an auto-regressive model for robotic control pre-trained on 4D human video representations, which lifts 2D keypoints into 3D via monocular depth to enable effective transfer from human videos to low-level robot tasks.'
date: 2025-5-1
venue: 'ICML'
paperurl: 'https://arxiv.org/abs/2502.13142'
website: 'https://arm4r.github.io/'
---
Dantong Niu<sup>\*</sup>, Yuvan Sharma<sup>\*</sup>, Haoru Xue, Giscard Biamby, Junyi Zhang, **Ziteng Ji**, Trevor Darrell, Roei Herzig

<sup>*</sup> (Equal contribution)

Foundation models pre-trained on massive unlabeled datasets have revolutionized natural language and computer vision, exhibiting remarkable generalization capabilities, thus highlighting the importance of pre-training. Yet, efforts in robotics have struggled to achieve similar success, limited by either the need for costly robotic annotations or the lack of representations that effectively model the physical world. In this paper, we introduce ARM4R, an Auto-regressive Robotic Model that leverages low-level 4D Representations learned from human video data to yield a better pre-trained robotic model. Specifically, we focus on utilizing 3D point tracking representations from videos derived by lifting 2D representations into 3D space via monocular depth estimation across time. These 4D representations maintain a shared geometric structure between the points and robot state representations up to a linear transformation, enabling efficient transfer learning from human video data to low-level robotic control. Our experiments show that ARM4R can transfer efficiently from human video data to robotics and consistently improves performance on tasks across various robot environments and configurations.
