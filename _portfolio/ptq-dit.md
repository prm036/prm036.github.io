---
title: "Post-Training Quantization (PTQ) for Diffusion Transformers"
collection: portfolio
excerpt: "Conducted an empirical study comparing FP and INT quantization formats on PixArt-α diffusion model."
---

Conducted a head-to-head empirical study, comparing low-bit floating-point (FP) and integer (INT) quantization formats on a **PixArt-α** (0.6B) diffusion model under similar precision budgets.

Observed that FP quantization yields better visual fidelity at low precision, improving **FID** from **42.4** to **38.8** under **W4A8** compared to INT PTQ with comparable **CLIP** and **ImageReward** scores.

[View on GitHub](https://github.com/prm036/DIT-PTQ/blob/main/report.pdf)
