---
layout: default
title: "Home"
---

Welcome to my Code Library! Here you can find resources, documentation, and more.

Feel free to explore and check out my repositories on GitHub.

For any questions or suggestions, you can email me.

<h1>Últimos Posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%d/%m/%Y" }}
    </li>
  {% endfor %}
</ul>
