---
layout: page
permalink: /people/
title: People
description: Here are all the cool people who work in the project!
nav: true
nav_order: 3
---

{% if site.data.people.people %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.people.people %}
    {% include people/person.html username=user.full_name description=user.description %}
  {% endfor %}
</div>
{% endif %}
