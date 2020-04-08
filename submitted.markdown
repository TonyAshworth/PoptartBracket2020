---
layout: page
title: Submitted Brackets
permalink: /submitted/
---

{% assign image_files = site.static_files | where: "bracket", true %}
{% for current_image in image_files %}

### {{current_image.basename}}

  [![]({{ current_image.path }})]({{ current_image.path }})

***

{% endfor %}