---
layout: page
title: Home
description: Listing of course modules
nav_order: 1
permalink: /
---

# **Data Science Mentors**

{: .mb-2 }
Spring 2025
{: .mb-2 .fs-6}

[Jump to Current Week](https://www.data8.org/fa24/#rrr-week){: .btn .btn-currweek}

{% include announcements-navigation.html %}

{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign active-mods = '' | split: '' %}

{% for mod in mods %}
  {% if mod.status == 'Active' %}
    {% assign active-mods = active-mods | push: mod %}
  {% endif %}
{% endfor %}

{% for module in active-mods %}
  {{ module }}
{% endfor %}

<script src="{{ '/assets/scripts/announcement-navigation.js' | relative_url }}"></script>