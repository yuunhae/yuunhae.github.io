---
title: "운영체제"
layout: category
permalink: /posts/operating-system/
category: operating-system
author_profile: true
sidebar_main: true
types: posts
# taxonomy:
#   category:
#     - computer-science
#     - operating-system
sidebar:
  nav: "sidebar-category"
  enabled: true
---
<!-- 
{% assign posts_with_computer-science = site.posts | where: "categories", "computer-science" %}
{% assign posts_with_computer-science_and_operating-system = posts_with_computer-science | where: "categories", "operating-system" %}

{% for post in posts_with_computer-science_and_operating-system %}
  {% include archive-single.html type=page.entries_layout %}
{% endfor %} -->

{% for post in site.categories.operating-system %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}