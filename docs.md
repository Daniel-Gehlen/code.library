---
layout: docs
title: Documentation
permalink: /docs/
---
<h2>Documentation</h2>

<div class="docs-sidebar">
  <h3>All Documents</h3>
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
