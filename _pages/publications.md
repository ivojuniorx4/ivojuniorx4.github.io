---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>JMP</h2>
{% for post in site.publications reversed %}
  {% if post.category == 'jmp' %}
    <!--<p>Debugging: {{ post.title }} - {{ post.category }}</p>-->
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

<!-- Add spacing -->
<br><be>

<h2>Working Papers</h2>
{% for post in site.publications reversed %}
  {% if post.category == 'working_paper' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
