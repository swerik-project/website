---
layout: page
permalink: /people/
title: Participants
description: ""
nav: true
nav_order: 2
---

{% if site.data.people.people %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.people.people %}
    {% include people/person.html username=user.full_name image=user.image description=user.description %}
  {% endfor %}
</div>
{% endif %}
