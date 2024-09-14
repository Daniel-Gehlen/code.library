---
layout: docs
title: Documentation
permalink: /docs/
---
<h1>Documentations</h1>

<div class="docs-sidebar">
  <h2>All Documents</h2>
  <ul>
    {% assign sorted_docs = site.docs | sort: 'title' %}
    {% for doc in sorted_docs %}
      <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
    {% endfor %}
  </ul>
</div>

<div class="docs-content">
  <p>Welcome to the documentation section. Click on the documents in the sidebar to read them.</p>
</div>
