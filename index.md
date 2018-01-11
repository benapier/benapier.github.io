---
title: Ben Napier
---

Hello
{{ post.data | date: "%B %e, %Y" }} <a href="{{ post.url {{">{{ post.title {{</a>

 <ul>
 -      {% for post in site.posts %}
 -      <li>
 -	<span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="{{ post.url }}">{{ post.title }}</a>
 -      </li>
 -      {% endfor %}
 -    </ul>
