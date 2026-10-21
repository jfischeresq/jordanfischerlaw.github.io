---
layout: page
title: Our Team
permalink: /ourteam/
wide: true
eyebrow: People
lede: "Experienced privacy, cybersecurity, and AI counsel who understand both the law and the business."
description: "Meet the attorneys of Fischer Law, P.C.."
---

<div class="grid grid-3">
{%- assign people = site.team | sort: "order" -%}
{%- for person in people -%}
  <a class="person" href="{{ person.url | relative_url }}">
    <img src="{{ person.image_path | uri_escape | relative_url }}" alt="Photo of {{ person.name }}" loading="lazy">
    <div class="person-body">
      <h3>{{ person.name }}</h3>
      {% if person.role %}<p>{{ person.role }}</p>{% endif %}
    </div>
  </a>
{%- endfor -%}
</div>
