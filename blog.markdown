---
layout: default
title: Blog
---

<div class="blog">
  <h1>Blog</h1>
  <p>Welcome to my blog! Here you'll find articles and updates on my projects and experiences.</p>
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
      </li>
    {% endfor %}
  </ul>
</div>
