---
layout: news
title: News
permalink: /news/
---

<h2>News page</h2>

<div class="news-sidebar">
  <h3>All news</h3>
  <ul>
    {% assign sorted_posts = site.posts | sort: 'date' %}
    {% for post in sorted_posts %}
      {% if post.categories contains 'news' %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="news-content">
  <p>Welcome to the news section. Click on the items in the sidebar to read more.</p>
</div>
