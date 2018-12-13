---
layout: default
---

## Bio

Student currently studying MSci Mathematics and Computer Science at Durham Universiy under the Millman Scholarship with the Materials Processing Institute.

## Current projects:

{% for page in site.projects %}
[{{ page.title }}]({{ page.url }})
{% endfor %}

## Resources:

{% for page in site.resources %}
[{{ page.title}}]({{ page.url }})
{% endfor %}
