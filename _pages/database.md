---
title: "데이터베이스"
layout: category
permalink: /posts/datebase/
author_profile: true
sidebar_main: true
types: posts
taxonomy:
  category:
    - computer-science
    - datebase
sidebar:
  nav: "sidebar-category"
  enabled: true
---

<!-- {% assign posts_with_computer-science = site.posts | where: "categories", "computer-science" %}
{% assign posts_with_computer-science_and_datebase = posts_with_computer-science | where: "categories", "datebase" %}

{% for post in posts_with_computer-science_and_datebase %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %} -->

{% for post in site.categories.database %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}