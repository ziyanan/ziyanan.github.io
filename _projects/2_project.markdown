---
layout: page
title: Formal Logic Enhanced AI and Deep Learning
description: How can formal specifications be integrated into learning-based AI to improve robustness, fairness, safety, and security in intelligent systems?
img: /assets/img/fig1enlarged1.png
importance: 1
category: Research at Vanderbilt
---

We proposed a federated learning training paradigm, called FedSTL, which enhances personalized client performance by encouraging model predictions to align with automatically inferred temporal logic properties. This approach enables collaboration among clients that share similar symbolic characteristics, improving robustness under heterogeneous and non-IID data distributions.

In addition, we incorporated signal temporal logic constraints to guide deep learning predictors toward fairer outputs. In this work, fairness properties related to demographic factors, such as age and median household income, were formally encoded for urban service allocation.

Building upon these contributions, my ongoing research extends the role of formal specifications from post-hoc analysis to a preventative security mechanism for cyber-physical systems. Specifically, I aim to develop a novel deep learning framework that integrates formal specifications into generative and diffusion-based models. This framework is designed to repair compromised or adversarially perturbed inputs by projecting them back onto the logical constraint set before downstream prediction. By embedding specification-driven correction into the learning pipeline, this approach moves beyond post-hoc detection toward proactive security, safety, and fairness guarantees in AI-enabled cyber-physical systems.

<h3 class="related-pubs-title">Related Publications</h3>
<ul class="related-pubs">
  <li>
    <span class="pub-title">Formal Logic-Guided Harnessing Heterogeneous Fairness Rules in Smart Cities</span><br>
    <strong>Ziyan An</strong>, Yiqi Zhao, Xuqing Gao, Ayan Mukhopadhyay, and Meiyi Ma<br>
    <em>ACM Transactions on Cyber-Physical Systems</em>, 2025
  </li>
  <li>
    <span class="pub-title">Formal Logic Enabled Personalized Federated Learning through Property Inference</span><br>
    <strong>Ziyan An</strong>, Taylor T. Johnson, and Meiyi Ma<br>
    <em>Proceedings of the AAAI Conference on Artificial Intelligence</em>, 2024
  </li>
  <li>
    <span class="pub-title">FairGuard: Harness Logic-Based Fairness Rules in Smart Cities</span><br>
    Yiqi Zhao, <strong>Ziyan An</strong>, Xuqing Gao, Ayan Mukhopadhyay, and Meiyi Ma<br>
    <em>Proceedings of the 8th ACM/IEEE Conference on Internet of Things Design and Implementation (IoTDI)</em>, 2023
  </li>
</ul>

<div class="row justify-content-center">
    <div class="col-md-7 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/fig1enlarged1.png' | relative_url }}" alt="FedSTL framework" title="FedSTL framework"/>
    </div>
</div>
<div class="caption">
    Figure 1: FedSTL infers temporal logic properties from each client's data, then uses them to group clients with similar behavior and guide aggregation and client selection during federated training.
</div>

<div class="row justify-content-center">
    <div class="col-md-10 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/train-deploy.png' | relative_url }}" alt="FairGuard training and deployment pipeline" title="FairGuard training and deployment pipeline"/>
    </div>
</div>
<div class="caption">
    Figure 2: The FairGuard pipeline combats unfair model behavior by incorporating fairness requirements during training and enforcing them through Static and Dynamic FairGuard, producing fair predictions at both training and deployment time.
</div>