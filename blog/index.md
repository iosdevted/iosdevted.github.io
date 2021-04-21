---
layout: default
work: true
main: true
title: Blog
description: "My passion and way to live a fulfilling life"
project-header: true
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.book == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>