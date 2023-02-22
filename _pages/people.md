---
layout: page
permalink: /people/
title: people
description: Here are all the cool people who work in the project!
nav: true
nav_order: 3
---

{% if site.data.people.full_names %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.people.full_names %}
    {% include people/person.html username=user %}
  {% endfor %}
</div>
{% endif %}
