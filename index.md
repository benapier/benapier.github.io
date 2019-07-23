---
layout: default
---

## Summary

Undergraduate Researcher with a demonstrated history of working in the research industry. Currently studying MSci Mathematics and Computer Science at Durham University under the Millman Scholarship with the Materials Processing Institute. 

[Coding activity](https://ben.napier.xyz/pages/coding_activity/)

## Current projects:

{% for page in site.projects %}
[{{ page.title }}]({{ page.url }})
{% endfor %}

## Resources:

{% for page in site.resources %}
[{{ page.title }}]({{ page.url }})
{% endfor %}
