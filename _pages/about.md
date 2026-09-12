---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* Hide the top masthead/header bar */
.masthead { display: none !important; }

.home-wrap { font-size: 0.82em; line-height: 1.7; }

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
.project-list { counter-reset: project-counter; }
.project-item { margin-bottom: 1.1em; counter-increment: project-counter; }
.project-item h4 {
  margin: 0 0 3px;
  font-size: 0.95em;
  font-weight: 700;
}
.project-item h4::before {
  content: counter(project-counter) ". ";
  color: #999;
  font-weight: 400;
}
.project-gh-link {
  font-size: 0.72em;
  font-weight: 400;
  color: #555;
  white-space: nowrap;
  text-decoration: none;
  display: inline-flex;
  align-items: center;
  gap: 3px;
  border: 1px solid #ccc;
  border-radius: 4px;
  padding: 1px 7px;
  margin-left: 7px;
  vertical-align: middle;
  line-height: 1.7;
  transition: border-color 0.15s, color 0.15s;
}
.project-gh-link:hover { color: #000; border-color: #888; text-decoration: none; }
.project-item p {
  margin: 0 0 3px;
  color: #444;
}

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
.exp-team { color: #999; font-style: italic; }
.exp-date { font-size: 0.82em; color: #999; white-space: nowrap; margin-left: 12px; }

.open-to-work { color: #c0392b; font-weight: 600; font-size: 0.9em; margin: 0.5em 0 0.8em; }
</style>

<div class="home-wrap">

<div class="section-heading">About</div>

<p>Hi, I'm Praneeth — a Master's student in Computer Science (MSCS) at <a href="https://www.northwestern.edu/">Northwestern University</a>, with concentration in Artificial Intelligence (expected Dec 2026).</p>

<p>I am broadly interested in <strong>Machine Learning</strong>, <strong>Foundation models</strong>, and <strong>Generative AI</strong>, particularly <a href="https://en.wikipedia.org/wiki/Diffusion_model">diffusion models</a>. I’m exploring these areas from both theoretical and a application perspective, focusing on developing models that are efficient, robust, and deployable in real-world environments.</p>

<p>Most recently, I interned at <a href="https://kilwa.io">Kilwa Technologies LLC</a> as an Machine Learning Engineer Intern, where I built hybrid time-series forecasting model for emerging african markets by combining macro-economic indicators and news-based sentiment signals. Prior to grad school, I was a Software Engineer at <a href="https://www.arcesium.com/">Arcesium</a> (D.E. Shaw Group), in the Infrastructure team building distributed job-execution systems, enterprise alerting systems and low-latency data-ingestion pipelines.</p>

<p>I'm currently looking for full-time roles in <strong>Machine Learning</strong> and <strong>Applied AI</strong> starting Jan 2027 — if you're working on something interesting, I'd love to connect. Feel free to reach out via <a href="mailto:praneeth.mallupalli@gmail.com">email</a>, <a href="https://www.linkedin.com/in/praneethreddym/">LinkedIn</a>, or <a href="https://github.com/prm036">GitHub</a>, or check out my <a href="/files/resume.pdf">CV</a>.</p>

<div class="section-heading">Projects</div>

<div class="project-list">

<div class="project-item">
  <h4>Fine-Tuning LLMs for Math Reasoning While Preserving Safety Alignment <a class="project-gh-link" href="https://github.com/prm036/fine-tuning-leads-to-forgetting/blob/main/report.pdf" target="_blank"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></h4>
  <p>Can you make an LLM better at math without breaking its safety guardrails? I fine-tuned <strong>Qwen2.5</strong> on <strong>GSM8K</strong> using <strong>LoRA</strong> and found that with the right setup, math accuracy jumps from 38% to 81% while the model still scores 88% on safety benchmarks. The trickier part was understanding when and why catastrophic forgetting kicks in — I ran ablations across 10 configurations to get a clearer picture.</p>
</div>

<div class="project-item">
  <h4>Post-Training Quantization (PTQ) for Diffusion Transformers <a class="project-gh-link" href="https://github.com/prm036/DIT-PTQ/blob/main/report.pdf" target="_blank"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></h4>
  <p>Diffusion models are powerful but expensive to run. I looked at whether floating-point or integer quantization holds up better when you aggressively compress <strong>PixArt-α</strong> to 4-bit weights and 8-bit activations. Turns out FP formats preserve visual quality noticeably better — FID dropped from 42.4 to 38.8 — while keeping CLIP and ImageReward scores on par.</p>
</div>

<div class="project-item">
  <h4>Deformable Object Manipulation with Vision-Language-Action Policies <a class="project-gh-link" href="https://github.com/prm036/Training-VLA-Policies-for-Deformable-Object-Manipulation-Tasks/blob/main/CS_396_Report.pdf" target="_blank"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></h4>
  <p>Teaching a robot to fold clothes is surprisingly hard — fabric doesn't behave predictably, and small errors compound quickly. I trained <strong>SmolVLA</strong> from teleoperated demos and got it to a 69% success rate on garment folding, beating both Diffusion Policy (41%) and ACT (61%). To boost generalization, we also trained it on synthetic data generated using NVIDIA's <strong>Cosmos-Transfer</strong>.</p>
</div>

<div class="project-item">
  <h4>Rotation Invariant Multi-Object Detector <a class="project-gh-link" href="https://github.com/prm036/Rotation-Invariant-Multi-Object-Detector/blob/main/Report.pdf" target="_blank"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></h4>
  <p>Standard object detectors quietly assume images are right-side up — flip or rotate a photo and accuracy tanks. I built a pre-processing step using eigenvector analysis that corrects image orientation before passing it to <strong>YOLOv3</strong>, with no retraining required. On Pascal VOC images rotated 90°–270°, this alone gave a 43% accuracy boost over a ResNet50 baseline.</p>
</div>

<div class="project-item">
  <h4>Deep RL for Real-Time Bidding in Sponsored Search &mdash; Literature Review <a class="project-gh-link" href="https://github.com/prm036/DRL-for-Real-Time-Bidding-RTB-in-Sponsored-Search/blob/main/report.pdf" target="_blank"><i class="fab fa-github" aria-hidden="true"></i> GitHub</a></h4>
  <p>Online ad auctions happen in milliseconds, and traditional rule-based bidders struggle to adapt to shifting market dynamics. This review surveys how Deep RL — specifically DQN variants — reframes real-time bidding as a constrained MDP and learns smarter budget-pacing strategies. The best approaches show up to 120% ROI gains over classical methods, though real-world deployment still has open challenges worth digging into.</p>
</div>

</div>

<div class="section-heading">Experience</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Machine Learning Intern</div>
    <div class="exp-company">Kilwa Technologies LLC &middot; <span class="exp-team">Time-series Forecasting for Emerging African Markets</span></div>
  </div>
  <span class="exp-date">Jun 2026 – Aug 2026</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Teaching Assistant</div>
    <div class="exp-company">Northwestern University &middot; <span class="exp-team">Machine Learning &amp; Sensing, Compiler Construction</span></div>
  </div>
  <span class="exp-date">Jan 2026 – Jun 2026</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Senior Software Engineer</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group) &middot; <span class="exp-team">Platform &amp; Distributed Systems</span></div>
  </div>
  <span class="exp-date">Jul 2023 – Aug 2025</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Software Engineer</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group) &middot; <span class="exp-team">Data Ingestion &amp; Log Infrastructure</span></div>
  </div>
  <span class="exp-date">Jun 2021 – Jun 2023</span>
</div>

<div class="exp-row">
  <div>
    <div class="exp-title">Data Science Intern</div>
    <div class="exp-company">Arcesium (D.E. Shaw Group) &middot; <span class="exp-team">Infrastructure Health &amp; Observability</span></div>
  </div>
  <span class="exp-date">Feb 2021 – May 2021</span>
</div>

</div>
