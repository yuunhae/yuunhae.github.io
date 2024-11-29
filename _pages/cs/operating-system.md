---
title: "운영체제"
layout: category
permalink: /cs/os/
author_profile: true
sidebar_main: true
types: posts
taxonomy:
  category:
    - cs
    - os
sidebar:
  nav: "sidebar-category"
  enabled: true
---

{% assign posts_with_cs = site.posts | where: "categories", "cs" %}
{% assign posts_with_cs_and_os = posts_with_cs | where: "categories", "os" %}

{% for post in posts_with_cs_and_os %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %}
