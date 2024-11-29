---
title: "컴퓨터 구조"
layout: category
permalink: /cs/architecture/
author_profile: true
sidebar_main: true
types: posts
taxonomy:
  category:
    - cs
    - architecture
sidebar:
  nav: "sidebar-category"
  enabled: true
---

{% assign posts_with_cs = site.posts | where: "categories", "cs" %}
{% assign posts_with_cs_and_architecture = posts_with_cs | where: "categories", "architecture" %}

{% for post in posts_with_cs_and_architecture %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
