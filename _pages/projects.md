---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

## Fine-Tuning LLMs for Math Reasoning While Preserving Safety Alignment
Fine-tuned **Qwen2.5** model(1.5B & 7B) on **GSM8K** dataset using **LoRA**, improving math accuracy to **0.81** while maintaining **0.88** safety alignment score on **AILuminate** Safety Dataset, surpassing baselines.

Performed ablation studies across **10** different hyperparameter configurations (learning rate, LoRA rank, dropout) to analyze performance trade-offs and mitigate catastrophic forgetting in fine-tuned models.

[View on GitHub](https://github.com/prm036/fine-tuning-leads-to-forgetting/blob/main/report.pdf)

---

## Post-Training Quantization (PTQ) for Diffusion Transformers
Conducted a head-to-head empirical study, comparing low-bit floating-point (FP) and integer (INT) quantization formats on a **PixArt-α** (0.6B) diffusion model under similar precision budgets.

Observed that FP quantization yields better visual fidelity at low precision, improving **FID** from **42.4** to **38.8** under **W4A8** compared to INT PTQ with comparable **CLIP** and **ImageReward** scores.

[View on GitHub](https://github.com/prm036/DIT-PTQ/blob/main/report.pdf)

---

## Deformable Object Manipulation with Vision-Language-Action Policies
Trained **SmolVLA** on teleoperated demonstrations using imitation learning for long-horizon control tasks, achieving **69%** success rate on garment folding, outperforming Diffusion Policy (**41%**) and ACT (**61%**) baselines.

Enhanced model generalization by augmenting training with NVIDIA **Cosmos-Transfer** synthetic data, exposing the policy to diverse physics-grounded visual scenarios.

[View on GitHub](https://github.com/prm036/Training-VLA-Policies-for-Deformable-Object-Manipulation-Tasks/blob/main/CS_396_Report.pdf)

---

## Rotation Invariant Multi-Object Detector
Addressed the limitations of traditional object detectors struggling to identify improperly oriented images by integrating eigenvector analysis and a custom decision criterion with a pre-trained **YOLOv3** model.

Achieved a **43%** accuracy improvement over the ResNet50 model on the Pascal VOC 2012 dataset for images deviated between **90°–270°**, without any rotation-augmented training.

[View on GitHub](https://github.com/prm036/Rotation-Invariant-Multi-Object-Detector/blob/main/Report.pdf)
