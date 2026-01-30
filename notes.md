---
title: "Notes"
permalink: /notes/
layout: single
---

Notes for courses and readings.

<ul>
{% for entry in site.data.files %}
  {% if entry.type == "notes" and entry.repo and entry.name %}
    <li>
      <a href="/files/{{ entry.repo }}.pdf">
        {{ entry.name }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>