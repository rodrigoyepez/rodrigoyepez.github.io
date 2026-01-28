---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

All publications are peer-reviewed and presented at IEEE International Conferences on Big Data.

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
