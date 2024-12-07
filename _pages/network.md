---
title: "컴퓨터 네트워크"
layout: category
permalink: /computer-science/network/
author_profile: true
sidebar_main: true
types: posts
taxonomy:
  category:
    - computer-science
    - network
sidebar:
  nav: "sidebar-category"
  enabled: true
---

{% assign posts_with_computer-science = site.posts | where: "categories", "computer-science" %}
{% assign posts_with_computer-science_and_network = posts_with_computer-science | where: "categories", "network" %}

{% for post in posts_with_computer-science_and_network %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
