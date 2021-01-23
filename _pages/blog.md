---
layout: archive
permalink: /blog/
title: "Blog posts"
author_profile: true
classes: wide
---

{% for post in site.posts %}
  {% include blog-single.html %}
{% endfor %}