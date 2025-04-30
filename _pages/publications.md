---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% if post.category == 'pub' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

#<br><be>

#<h2>Working Papers</h2>
#{% for post in site.publications reversed %}
#  {% if post.category == 'working_paper' %}
#    {% include archive-single.html %}
#  {% endif %}
#{% endfor %}
