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

* **Using Intelligent Conversational Agents to Empower Adolescents to be Resilient Against Cybergrooming**

  * Funding: National Science Foundation (NSF)
  * Dates: Fall 2024 - Present
  * Principal Investigators: Jin-Hee Cho, Pamela J. Wisniewski, Lifu Huang, Sang Won Lee
  * Website: [Link](https://wordpress.cs.vt.edu/rylai/)
* **AI-Powered Solution for Cyber Scam Prevention: Empowering Community Support for Older Adults**

  * Funding: Commonwealth Cyber Initiative (CCI) and OpenAI
  * Dates: Fall 2025 - Present
  * Principal Investigators: Jin-Hee Cho, Junghwan Kim


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
