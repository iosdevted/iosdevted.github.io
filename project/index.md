---
layout: default
work: true
main: true
title: Project
description: "All the Apps I've worked on"
project-header: true
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.projects == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
