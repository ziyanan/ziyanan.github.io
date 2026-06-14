---
layout: page
title: Runtime Monitoring of AI-enabled Systems
description: How can symbolic reasoning and formal logic provide runtime insight into model behavior, performance, and anomalies under real-world variability?
img: /assets/img/fig1-2.png
importance: 3
category: Research at Vanderbilt
card_min_height: 220px
---

To provide insight into specification satisfaction under uncertainty, we developed a logic-based monitoring framework for traffic safety that analyzes dashboard camera streams using temporal specifications. This framework detects dangerous driving behaviors and accidents beyond traditional accuracy metrics.

In smart health applications, we introduced a formal specification logic for medical image segmentation to qualitatively and quantitatively assess model outputs against anatomical and topological constraints. This approach enables structured reasoning about anatomical consistency rather than relying solely on pixel-level accuracy.

Building upon these contributions, my ongoing research aims to extend formal specifications into richer temporal domains. Specifically, I seek to monitor data-driven segmentation models over time, enabling reasoning about temporal consistency and structural integrity in continuous data streams. For example, the framework will be able to detect violations where a segment in one frame shifts significantly in the next frame, indicating instability or potential model failure. By incorporating temporal logic into segmentation and perception monitoring, this work advances reasoning about deep learning models in dynamic cyber-physical system environments, such as driving and smart health systems.

<h3 class="related-pubs-title">Related Publications</h3>
<ul class="related-pubs">
  <li>
    <span class="pub-title">ISL: Monitoring Image Segmentation Logic in Medical Imaging Analysis</span><br>
    <strong>Ziyan An</strong>, Daniel Moyer, Ipek Oguz, Taylor T. Johnson, and Meiyi Ma<br>
    <em>International Conference on Runtime Verification</em>, 2025
  </li>
  <li>
    <span class="pub-title">Formal Logic-Guided Harnessing Heterogeneous Fairness Rules in Smart Cities</span><br>
    <strong>Ziyan An</strong>, Yiqi Zhao, Xuqing Gao, Ayan Mukhopadhyay, and Meiyi Ma<br>
    <em>ACM Transactions on Cyber-Physical Systems</em>, 2025
  </li>
  <li>
    <span class="pub-title">Runtime Monitoring of Accidents in Driving Recordings with Multi-Type Logic in Empirical Models</span><br>
    <strong>Ziyan An</strong>, Xia Wang, Taylor T. Johnson, Jonathan Sprinkle, and Meiyi Ma<br>
    <em>International Conference on Runtime Verification</em>, 2023
  </li>
</ul>

<div class="row justify-content-center">
    <div class="col-md-12 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/fig1-2.png' | relative_url }}" alt="Runtime accident monitoring pipeline" title="Runtime accident monitoring pipeline"/>
    </div>
</div>
<div class="caption">
    Figure 1: The runtime monitoring pipeline processes dashboard camera streams and evaluates them against multi-type logic specifications (FOL, HOL, STL) to detect dangerous driving behaviors and accidents on the fly.
</div>

<div class="row justify-content-center">
    <div class="col-md-9 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/isl-overview.png' | relative_url }}" alt="Image Segmentation Logic (ISL) monitoring overview" title="Image Segmentation Logic (ISL) monitoring overview"/>
    </div>
</div>
<div class="caption">
    Figure 2: Image Segmentation Logic (ISL) augments a U-Net segmentation model's outputs into a structured representation, then monitors them against pixel- and region-level logic formulas that encode anatomical and topological constraints.
</div>
