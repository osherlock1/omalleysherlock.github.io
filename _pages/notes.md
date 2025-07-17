---
layout: archive
title: "Notes"
permalink: /notes/
---

{% for note in site.notes %}
- [{{ note.title | default: note.path | split: '/' | last | replace: '.md', '' }}]({{ note.url }})
{% endfor %}
