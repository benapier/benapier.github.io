---
layout: default
---

# Current projects:

{% for page in site.pages %}
{{ page.title }}
{% endfor %}

# Posts

<!-- {% for post in site.posts %}
* {{ post.date | date_to_long_string }}, [{{ post.title }}]({{ post.url }})
{% endfor %} -->
