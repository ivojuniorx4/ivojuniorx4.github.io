---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---


You can also find my articles on <u><a href="https://scholar.google.com/citations?user=vFMsAHcAAAAJ&hl=en">my Google Scholar profile</a>.</u>

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% if post.category == 'published_paper' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
