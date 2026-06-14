---
layout: page
title: Projects and Thrusts
permalink: /projects/
description:
nav: true
nav_order: 2
display_categories: [Research at Vanderbilt, Research at NYU]
horizontal: true
---
<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
    {% for category in page.display_categories %}
      <h2 class="category">{{category}}</h2>
      {% if category == "Research at Vanderbilt" %}
      <div class="project-intro">
        <h3>Introduction and Motivation</h3>
        <p>Modern cyber-physical systems (CPS) are increasingly deployed in safety-critical domains such as intelligent transportation, smart cities, healthcare, and distributed infrastructure. These systems often require human intervention and interdisciplinary expertise spanning urban planning and design, control theory, transportation engineering, and public policy. As the field moves toward broader deployment of AI in CPS, data-driven learning algorithms are being integrated to support perception, prediction, and decision-making tasks.</p>
        <p>Despite AI models achieving strong performance during development, their real-world adoption in safety-critical settings remains limited. Practitioners often raise concerns about trust, model behavior under uncertainty, lack of transparency, and the difficulty of verifying learned components. These challenges hinder the reliable deployment of AI in CPS. Moreover, empirical accuracy alone is insufficient when uncertainties arise during deployment and decisions affect real-world safety and public infrastructure. In such cases, systems must also demonstrate reliability, interpretability, and guarantees.</p>
        <p>Addressing these limitations requires embedding formal specification and reasoning mechanisms directly into learning-based AI. Formal methods provide mathematically grounded frameworks for specifying and rigorously verifying system behavior, thereby mitigating risks associated with undesired or unsafe outputs. Additionally, specification languages such as temporal logic can guide the design and training of learning-based AI. By encoding domain constraints directly into the learning process, these methods shape model behavior toward safer, more robust, and more aligned decision-making, rather than relying solely on post-hoc validation.</p>
        <p>Building on this foundation, my research also emphasizes improving human understanding of AI decision-making. Logic-guided explanation mechanisms are developed to translate formal properties into rigorous yet accessible interpretations for stakeholders. Overall, my research seeks to balance theoretical rigor with practical deployment, with applications in traffic prediction, transit planning, and smart city systems, including collaborations with local Tennessee public transit agencies.</p>
      </div>
      {% endif %}
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <!-- Generate cards for each project -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-1">
          {% for project in sorted_projects %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for project in sorted_projects %}
            {% include projects.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display projects without categories -->
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for project in sorted_projects %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_projects %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>
