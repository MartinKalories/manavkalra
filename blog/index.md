---
layout: default
title: Blog
---

<section class="page-intro">
  <p style="margin:0; color:#4f46e5; font-weight:700; letter-spacing:0.14em; text-transform:uppercase;">Latest posts</p>
  <h1>Blog</h1>
  <p>Thoughtful updates on what I’m learning, building, and planning next. These posts show active progress and practical ideas.</p>
</section>

<ul class="blog-list">
  {% for post in site.posts %}
    <li class="blog-item">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <time>{{ post.date | date: "%B %d, %Y" }}</time>
      <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
    </li>
  {% endfor %}
</ul>