---
layout: default
title: Home
---

# Hi, I'm Yash 👋  
Student • Developer • Ireland  

Welcome to **baroot.me** — my space for writing about code, tech, and life.

---

## Latest Posts

<ul class="post-list">
  {% for post in site.posts limit:5 %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
      </h3>
      <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </li>
  {% endfor %}
</ul>

<p><a href="/archive">View all posts →</a></p>
