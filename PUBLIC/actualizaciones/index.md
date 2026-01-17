---
layout: default
title: Actualizaciones DSR Labs
---

# Actualizaciones DSR Labs

{% for file in site.static_files %}
  {% if file.path contains "/PUBLIC/actualizaciones/"
        and file.extname == ".md"
        and file.name != "index.md" %}
- [{{ file.name | replace: "_", " " | replace: ".md", "" }}]({{ file.name }})
  {% endif %}
{% endfor %}