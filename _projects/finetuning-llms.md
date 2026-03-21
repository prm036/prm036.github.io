---
title: "Fine-Tuning LLMs for Math Reasoning While Preserving Safety Alignment"
collection: projects
excerpt: "Fine-tuned Qwen2.5 on GSM8K dataset using LoRA, improving math accuracy while maintaining safety alignment."
---

Fine-tuned **Qwen2.5** model(1.5B & 7B) on **GSM8K** dataset using **LoRA**, improving math accuracy to **0.81** while maintaining **0.88** safety alignment score on **AILuminate** Safety Dataset, surpassing baselines.

Performed ablation studies across **10** different hyperparameter configurations (learning rate, LoRA rank, dropout) to analyze performance trade-offs and mitigate catastrophic forgetting in fine-tuned models.

[View on GitHub](https://github.com/prm036/fine-tuning-leads-to-forgetting/blob/main/report.pdf)
