---
layout: default
title: 2nd Semester
permalink: /semester2/
---

<style>
  .sem-title { font-size: 2.5rem; font-weight: 700; margin: 3rem 0 0.5rem 0; }
  .sem-label { font-size: 0.75rem; letter-spacing: 0.15em; text-transform: uppercase; opacity: 0.5; }
  .post-list { list-style: none; padding: 0; margin-top: 3rem; }
  .post-item { padding: 2rem 0; border-top: 1px solid rgba(0,0,0,0.1); }
  .post-item a { font-size: 1.4rem; font-weight: 600; text-decoration: none; color: inherit; }
  .post-item a:hover { opacity: 0.6; }
  .post-date { font-size: 0.8rem; opacity: 0.4; margin-top: 0.3rem; }
</style>

<p class="sem-label">First Year · 2025-2026</p>
<h1 class="sem-title">2nd Semester</h1>

<ul class="post-list">
  {% for post in site.posts %}
    {% if post.semester == "second" %}
    <li class="post-item">
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    </li>
    {% endif %}
  {% endfor %}
</ul>
