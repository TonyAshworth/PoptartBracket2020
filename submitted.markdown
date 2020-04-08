---
layout: page
title: Submitted Brackets
permalink: /submitted/
---

{% assign image_files = site.static_files | where: "bracket", true %}
{% for current_image in image_files %}

### {{current_image.basename}}

  [![]({{ site.baseurl }}{{ current_image.path }})]({{ site.baseurl }}{{ current_image.path }})

***

{% endfor %}