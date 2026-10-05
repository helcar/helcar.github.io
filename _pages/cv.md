---
layout: archive
title: " "
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

Education
=========

* Ph.D in Computer Science, Virginia Tech, 2026 (expected)
* M.S. in Computer Science, New York University, 2021
* B.S. in Electronic Science and Technology, Beijing Institute of Technology, 2019

<!-- Work Experience
=============== -->


Research Projects
=================

  * **Strategic and Stage-Structured LLM Dialogue Systems**
    * Funding: National Science Foundation (NSF)
    * Date: Sep. 2024 – Present
    * Principal Investigators: Jin-Hee Cho, Pamela J. Wisniewski, Lifu Huang, Sang Won Lee
    * Website: [Link](https://wordpress.cs.vt.edu/rylai/)
    * Investigate how large language models can conduct structured, goal-directed, and long-horizon conversations in socially sensitive domains.
    * Developed **DeepSAGE**, a hybrid LLM–Deep Reinforcement Learning framework that models an initial Cognitive Behavioral Therapy session as eleven stages with explicit therapeutic objectives.
    * Contributed to **StagePilot**, an offline reinforcement learning framework for stage-controlled cybergrooming dialogue simulation.


  * **Detection, Explanation, and Mitigation of AI Failures**
    * Funding: National Science Foundation (NSF)
    * Date: Aug. 2025 – Present
    * Principal Investigators: Jin-Hee Cho
    * Website: [Link](https://wordpress.cs.vt.edu/rylai/)
    * Study trustworthy AI from an instance-level perspective, focusing on detecting, explaining, prioritizing, and mitigating individual model failures after deployment.
    * Developed **X-MAP**, an explainable misclassification-analysis framework that transforms local SHAP attributions into semantic topic profiles using non-negative matrix factorization.

  * **Uncertainty-Aware Reinforcement Learning for Competitive Influence Maximization**
    * Funding: National Science Foundation (NSF)
    * Date: Oct. 2021 – Aug. 2025
    * Principal Investigators: Jin-Hee Cho, Feng Chen, Dong Hyun Jeong
    * Investigated competitive influence maximization under uncertain, evolving, and non-binary user opinions.
    * Developed **DRIM**, a dual-agent Deep Reinforcement Learning framework for modeling strategic competition between parties propagating true and false information in online social networks.


Teaching Experience
===================

* **Virginia Tech** (Teaching Assistant)
  * CS 5584: Network Security — Fall 2026
  * CS 2104: Introduction to Problem Solving in Computer Science — Spring 2022, Summer 2024
  * CS 3114: Data Structures and Algorithms — Fall 2021

* **New York University** (Teaching Assistant)
  * CS-GY 6823: Network Security — Spring 2021

Publications
============

<ul>
{% assign pubs = site.publications | sort: "date" | reverse %}
{% for post in pubs %}
  <li>{{ post.citation }}{% if post.paperurl %} <a href="{{ post.paperurl }}">[Link]</a>{% endif %}</li>
{% endfor %}
</ul>

Talks
=====

<ul>
{% assign talks = site.talks | sort: "date" | reverse %}
  {% for post in talks %}
    <li>
      <strong>{{ post.title }}</strong>,
      {{ post.venue }}{% if post.location %}, {{ post.location }}{% endif %},
      {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
