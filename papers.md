---
title: "Papers"
permalink: /papers/
layout: single
---


## Papers


<ul>
{% for entry in site.data.files %}
  {% if entry.type == "paper" and entry.repo and entry.name %}
    <li>
      <a href="/files/{{ entry.repo }}.pdf">
        {{ entry.name }}
      </a>
    </li>
  {% endif %}
{% endfor %}
</ul>