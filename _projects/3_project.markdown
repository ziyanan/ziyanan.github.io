---
layout: page
title: Trustworthy and Explainable AI
description: Leverage the rigor of logic and translate verified logic evidence into faithful, human-centered explanations for complex AI outcomes.
img: /assets/img/xai.png
importance: 2
category: Research at Vanderbilt
---

We developed a Computation Tree Logic (CTL)-based explainer for Monte Carlo Tree Search (MCTS) in sequential transit planning. The method converts user queries into formal logic specifications, evaluates them over the search tree using CTL semantics, and returns semantically grounded explanations.

Building on this, we introduced LogiEx, a logic-integrated explanation framework that combines formal verification with large language models (LLMs) to interpret complex MCTS trees. LogiEx supports free-form queries, human-guided search exploration, and logic-grounded explanations, while ensuring faithfulness by validating responses against the underlying planning process.

My research further establishes a framework for reliable, verifiable, and human-centered explanations in complex planning systems across additional real-time domains. Future work will focus on deploying and evaluating this framework in collaboration with the Williamson County Department of Transportation, with the goal of addressing community concerns regarding school bus routing and scheduling decisions and assessing its effectiveness in real-world operational settings.

<h3 class="related-pubs-title">Related Publications</h3>
<ul class="related-pubs">
  <li>
    <span class="pub-title">LogiEx: Integrating Formal Logic and LLMs for Explainable Transit Planning</span><br>
    <strong>Ziyan An</strong>, Xia Wang, Hendrik Baier, Zirong Chen, Abhishek Dubey, Taylor T. Johnson, Jonathan Sprinkle, and Meiyi Ma<br>
    <em>Proceedings of the 17th ACM/IEEE International Conference on Cyber-Physical Systems (ICCPS)</em>, 2026
  </li>
  <li>
    <span class="pub-title">X-CPS: A Top-Down Hierarchical Framework for Explaining Learning-enabled Cyber-Physical Systems</span><br>
    Guocheng He, Lingwen Deng, <strong>Ziyan An</strong>, and Meiyi Ma<br>
    <em>The 3rd International Workshop on Foundation Models for Cyber-Physical Systems &amp; Internet of Things (FMSys'26), CPS-IoT Week</em>, 2026
  </li>
  <li>
    <span class="pub-title">Combining LLMs with Logic-Based Framework to Explain MCTS</span><br>
    <strong>Ziyan An</strong>, Xia Wang, Hendrik Baier, Zirong Chen, Abhishek Dubey, Taylor T. Johnson, Jonathan Sprinkle, Ayan Mukhopadhyay, and Meiyi Ma<br>
    <em>The 24th International Conference on Autonomous Agents and Multi-Agent Systems (AAMAS)</em>, 2025
  </li>
  <li>
    <span class="pub-title">Enabling MCTS Explainability for Sequential Planning through Computation Tree Logic</span><br>
    <strong>Ziyan An</strong>, Hendrik Baier, Abhishek Dubey, Ayan Mukhopadhyay, and Meiyi Ma<br>
    <em>European Conference on Artificial Intelligence (ECAI)</em>, 2024
  </li>
</ul>

<div class="row justify-content-center">
    <div class="col-md-9 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/xai.png' | relative_url }}" alt="Logic-guided explanation for transit planning" title="Logic-guided explanation for transit planning"/>
    </div>
</div>
<div class="caption">
    Figure 1: A domain expert selects from a set of predefined checkbox queries about a transit plan. A CTL-based framework then evaluates the selected query over the planning search tree through a CTL checking process, and the explanation framework converts the CTL checking outputs into templated, human-readable results.
</div>

<div class="row justify-content-center">
    <div class="col-md-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/logiex-overview.png' | relative_url }}" alt="LogiEx Planning Explainer overview" title="LogiEx Planning Explainer overview"/>
    </div>
</div>
<div class="caption">
    Figure 2: The LogiEx Planning Explainer sits between the MCTS-based transit planner and a domain expert, interpreting the search process to answer free-form questions with logic-grounded, faithful responses validated against the underlying plan.
</div>