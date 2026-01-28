---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

A selection of my machine learning and data science projects.

{% for post in site.portfolio reversed %}
  {% include archive-single.html %}
{% endfor %}
