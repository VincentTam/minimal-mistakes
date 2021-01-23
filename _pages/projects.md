---
title: "Projects"
layout: archive
permalink: /projects/
collection: projects
author_profile: true
classes: wide
---

{% for post in site.projects reversed %}
    {% include project-single.html %}
{% endfor %}