---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.home-wrap { font-size: 0.87em; line-height: 1.7; }

.section-heading {
  font-size: 1em;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.07em;
  color: #555;
  border-bottom: 1px solid #ddd;
  padding-bottom: 3px;
  margin: 1.8em 0 0.9em;
}

/* Projects */
.project-item { margin-bottom: 1.1em; }
.project-item h4 {
  margin: 0 0 3px;
  font-size: 0.95em;
  font-weight: 700;
}
.project-item p {
  margin: 0 0 3px;
  color: #444;
  font-size: 0.9em;
}
.project-item a { font-size: 0.85em; color: #0077aa; }

/* Experience */
.exp-row {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  padding: 5px 0;
  border-bottom: 1px solid #f2f2f2;
}
.exp-row:last-child { border-bottom: none; }
.exp-title { font-weight: 600; font-size: 0.9em; }
.exp-company { color: #666; font-size: 0.85em; }
.exp-date { font-size: 0.82em; color: #999; white-space: nowrap; margin-left: 12px; }

.open-to-work { color: #c0392b; font-weight: 600; font-size: 0.9em; margin: 0.5em 0 0.8em; }
</style>

<div class="home-wrap">

<p>Hi, I'm Praneeth — a Master's student in Computer Science (MSCS) at <a href="https://www.northwestern.edu/">Northwestern University</a>, with concentration in Artificial Intelligence (expected Dec 2026).</p>

<p>I am broadly interested in <strong>Machine Learning</strong>, <strong>Foundation models</strong>, and <strong>Generative AI</strong>, particularly <a href="https://en.wikipedia.org/wiki/Diffusion_model">diffusion models</a>. I’m exploring these areas from both theoretical and a application perspective, focusing on developing models that are efficient, robust, and deployable in real-world environments.</p>

<p>Previously, I worked as a Software Engineer at <a href="https://www.arcesium.com/">Arcesium</a>, building distributed systems and data-ingestion pipelines.</p>

<p class="open-to-work">I am actively looking for full-time opportunities in Machine Learning and Applied AI areas starting Jan 2027.</p>

<p>Reach out via <a href="mailto:praneeth.mallupalli@gmail.com">email</a>, <a href="https://www.linkedin.com/in/praneethreddym/">LinkedIn</a>, or <a href="https://github.com/prm036">GitHub</a>. View my <a href="/files/resume.pdf">CV</a> for more details.</p>

<div class="section-heading">Projects</div>

<div class="project-item">
  <h4>Fine-Tuning LLMs for Math Reasoning While Preserving Safety Alignment</h4>
  <p>Fine-tuned <strong>Qwen2.5</strong> (1.5B &amp; 7B) on <strong>GSM8K</strong> via <strong>LoRA</strong> — math accuracy 38% → 81%, safety score 88%. Ablation across 10 configs to study catastrophic forgetting.</p>
  <a href="https://github.com/prm036/fine-tuning-leads-to-forgetting/blob/main/report.pdf">GitHub</a>
</div>

<div class="project-item">
  <h4>Post-Training Quantization (PTQ) for Diffusion Transformers</h4>
  <p>Compared FP vs INT low-bit quantization on <strong>PixArt-α</strong> (0.6B). FP improved FID 42.4 → 38.8 under <strong>W4A8</strong> with comparable CLIP and ImageReward scores.</p>
  <a href="https://github.com/prm036/DIT-PTQ/blob/main/report.pdf">GitHub</a>
</div>

<div class="project-item">
  <h4>Deformable Object Manipulation with Vision-Language-Action Policies</h4>
  <p>Trained <strong>SmolVLA</strong> via imitation learning for garment folding — 69% success, outperforming Diffusion Policy (41%) and ACT (61%). Augmented with NVIDIA <strong>Cosmos-Transfer</strong> synthetic data.</p>
  <a href="https://github.com/prm036/Training-VLA-Policies-for-Deformable-Object-Manipulation-Tasks/blob/main/CS_396_Report.pdf">GitHub</a>
</div>

<div class="project-item">
  <h4>Rotation Invariant Multi-Object Detector</h4>
  <p>Combined eigenvector analysis with <strong>YOLOv3</strong> to handle rotated images. 43% accuracy improvement over ResNet50 on Pascal VOC 2012 (90°–270°), without rotation-augmented training.</p>
  <a href="https://github.com/prm036/Rotation-Invariant-Multi-Object-Detector/blob/main/Report.pdf">GitHub</a>
</div>

<div class="project-item">
  <h4>Deep RL for Real-Time Bidding in Sponsored Search &mdash; Literature Review</h4>
  <p>Analyzed DRL-based RTB as a constrained MDP. Compared DQN architectures on budget-pacing, finding up to 120% ROI improvement over traditional bidding methods.</p>
  <a href="https://github.com/prm036/DRL-for-Real-Time-Bidding-RTB-in-Sponsored-Search/blob/main/report.pdf">GitHub</a>
</div>

<div class="section-heading">Experience</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Teaching Assistant</div>
    <div class="exp-company">Northwestern University</div>
  </div>
  <span class="exp-date">Jan 2026 – Present</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Senior Software Engineer</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group)</div>
  </div>
  <span class="exp-date">Jul 2023 – Aug 2025</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Software Engineer</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group)</div>
  </div>
  <span class="exp-date">Jun 2021 – Jun 2023</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Data Science Intern</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group)</div>
  </div>
  <span class="exp-date">Feb 2021 – May 2021</span>
</div>

</div>
