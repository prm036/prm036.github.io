---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div style="font-size: 0.88em; line-height: 1.6;">

Hi, I'm Praneeth — a Master's student in Computer Science (MSCS) at <a href="https://www.northwestern.edu/">Northwestern University</a>, specializing in Artificial Intelligence (expected Dec 2026).

I am broadly interested in **Machine Learning**, **Foundation models**, and **Generative AI**, particularly <a href="https://en.wikipedia.org/wiki/Diffusion_model">diffusion models</a>. I'm exploring these areas from both a theoretical and a systems/application perspective, focusing on developing models that are not only high-performing, but also efficient and deployable in real-world environments.

Before starting my master's, I was a Software Engineer at <a href="https://www.arcesium.com/">Arcesium</a>, where I worked on distributed systems, including job-execution engines and data-ingestion pipelines.

<p style="color: red; font-weight: 600; margin-top: 6px;">I am actively looking for full-time opportunities in Machine Learning and Applied AI areas starting Jan 2027.</p>

Reach out via <a href="mailto:praneeth.mallupalli@gmail.com">email</a>, <a href="https://www.linkedin.com/in/praneethreddym/">LinkedIn</a>, or <a href="https://github.com/prm036">GitHub</a>. You can also view my <a href="/files/resume.pdf">CV</a> for more details.

---

## Projects

### Fine-Tuning LLMs for Math Reasoning While Preserving Safety Alignment
Fine-tuned **Qwen2.5** models (1.5B & 7B) on the **GSM8K** dataset using **LoRA**, improving math accuracy from 38% to 81% while maintaining a strong 88% safety alignment score on the **AILuminate** Safety Dataset.

Performed ablation studies across **10** different hyperparameter configurations (learning rate, LoRA rank, dropout) to analyze performance trade-offs and mitigate catastrophic forgetting in fine-tuned models.

<a href="https://github.com/prm036/fine-tuning-leads-to-forgetting/blob/main/report.pdf">View on GitHub</a>

---

### Post-Training Quantization (PTQ) for Diffusion Transformers
Conducted a head-to-head empirical study, comparing low-bit floating-point (FP) and integer (INT) quantization formats on a **PixArt-α** (0.6B) diffusion model under similar precision budgets.

Observed that FP quantization yields better visual fidelity at low precision, improving **FID** from **42.4** to **38.8** under **W4A8** compared to INT PTQ with comparable **CLIP** and **ImageReward** scores.

<a href="https://github.com/prm036/DIT-PTQ/blob/main/report.pdf">View on GitHub</a>

---

### Deformable Object Manipulation with Vision-Language-Action Policies
Trained **SmolVLA** on teleoperated demonstrations using imitation learning for long-horizon control tasks, achieving **69%** success rate on garment folding, outperforming Diffusion Policy (**41%**) and ACT (**61%**) baselines.

Enhanced model generalization by augmenting training with NVIDIA **Cosmos-Transfer** synthetic data, exposing the policy to diverse physics-grounded visual scenarios.

<a href="https://github.com/prm036/Training-VLA-Policies-for-Deformable-Object-Manipulation-Tasks/blob/main/CS_396_Report.pdf">View on GitHub</a>

---

### Rotation Invariant Multi-Object Detector
Addressed the limitations of traditional object detectors struggling to identify improperly oriented images by integrating eigenvector analysis and a custom decision criterion with a pre-trained **YOLOv3** model.

Achieved a **43%** accuracy improvement over the ResNet50 model on the Pascal VOC 2012 dataset for images deviated between **90°–270°**, without any rotation-augmented training.

<a href="https://github.com/prm036/Rotation-Invariant-Multi-Object-Detector/blob/main/Report.pdf">View on GitHub</a>

---

### Deep Reinforcement Learning for Real-Time Bidding (RTB) in Sponsored Search: A Literature Review
Analyzed Deep Reinforcement Learning (DRL) applications in Real-Time Bidding (RTB), formulating the bidding process as a constrained Markov Decision Process (MDP) to address highly non-stationary market behaviors.

Evaluated Deep Q-Network (DQN) architectures — comparing Control-by-Model state aggregation against Direct-Action continuous adaptation — highlighting strategies that improve long-term budget pacing and achieve up to a 120% ROI increase over traditional ones.

<a href="https://github.com/prm036/DRL-for-Real-Time-Bidding-RTB-in-Sponsored-Search/blob/main/report.pdf">View on GitHub</a>

---

## Experience

**Peer Mentor (Teaching Assistant)** | *Northwestern University*, Evanston, IL _(Jan 2026 – Present)_
* [**Machine Learning and Sensing**](https://www.mccormick.northwestern.edu/computer-science/academics/courses/descriptions/396-496-22.html) (Prof. Karan Ahuja) — Spring '26
* [**Compiler Construction**](https://www.mccormick.northwestern.edu/computer-science/academics/courses/descriptions/322.html) (Prof. Dietrich Geisler) — Winter '26
* Facilitated weekly office hours and supported students through assignments and projects throughout the quarter.
* Graded coding assignments and projects, providing detailed and constructive feedback.
* Coordinated course logistics, including inviting and scheduling external guest speakers.

**Senior Software Engineer** | *Arcesium (D.E. Shaw Group)*, Hyderabad, India _(July 2023 – Aug 2025)_
* Optimized the executor component of a **distributed job execution engine** (1M+ jobs/day) by caching eligible jobs metadata at the host-level, resulting in a 70% reduction in DynamoDB reads, and enabling dynamic autoscaling.
* Developed a domain-aware alert aggregation feature for a large-scale alerting system, improving efficiency by **30%**.
* Secured APIs with **HMAC verification**, blocking 100% of unauthorized traffic while maintaining less than 0.5ms latency.

**Software Engineer** | *Arcesium (D.E. Shaw Group)*, Hyderabad, India _(June 2021 – June 2023)_
* Designed a backend service orchestrating a high-throughput log ingestion pipeline (40TB/day) with zero data loss.
* Developed a configuration-driven routing module that dynamically maps logs to Kafka topics and Elasticsearch indices using schema-aware rules and declarative configs.

**Data Science Intern** | *Arcesium (D.E. Shaw Group)*, Hyderabad, India _(Feb 2021 – May 2021)_
* Designed a statistical model to compute health scores for core infrastructure services by normalizing multi-source service metrics (1M+ data points/day) of non-uniform ranges.
* Leveraged ETS time-series models to capture trends and anomalies, improving health prediction accuracy by **30%** over heuristic methods.

---

## Coursework

#### Fall 2025
* **COMP_SCI 358**: Parallel Computing
* **COMP_SCI 349**: Machine Learning
* **COMP_SCI 437**: Approximation Algorithms

#### Winter 2026
* **IEMS 490**: Deep Generative AI
* **COMP_SCI 449**: Deep Learning
* **ELEC_ENG 473**: Deep Reinforcement Learning from Scratch
* **COMP_SCI 396**: Reasoning and Planning in the Foundation Model Era

#### Spring 2026
* **COMP_SCI 496**: Agent AI
* **COMP_SCI 461**: Deep Learning for Natural Language Processing
* **IEMS 305**: Foundations of Modern Machine Learning
* **IEMS 490**: Advanced Topics in Large Foundation Models

</div>
