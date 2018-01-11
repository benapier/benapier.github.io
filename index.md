---
layout: default
---

### Description

Motivated and organised student with a strong foundation in computer science and interests
in a wide range of topics.

### Current projects:

{% for page in site.pages %}
[{{ page.title }}]({{ page.url }})
Dog
{% endfor %}

### Posts

<!-- {% for post in site.posts %}
* {{ post.date | date_to_long_string }}, [{{ post.title }}]({{ post.url }})
{% endfor %} -->
