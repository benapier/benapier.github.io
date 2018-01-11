---
layout: default
---

## Bio

Motivated and organised student with a strong foundation in computer science and interests
in a wide range of topics.

## Current projects:

{% for page in site.projects %}
[{{ page.title }}]({{ page.url }})
{% endfor %}
