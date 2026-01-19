---
layout: default
title: Arquitectura DSR Labs
---

# Arquitectura DSR Labs

{% for file in site.static_files %}
  {% if file.path contains "/SYSTEMS/arquitectura/"
        and file.extname == ".md"
        and file.name != "index.md" %}
- [{{ file.name | replace: "_", " " | replace: ".md", "" }}]({{ file.name }})
  {% endif %}
{% endfor %}