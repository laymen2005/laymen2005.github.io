---
layout: page
title: "古文鉴赏"
permalink: /marks/
---

### 全部古文列表

<ul class="post-list">
  {% for post in site.categories.marks %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title }}
        </a>
      </h3>
    </li>
  {% endfor %}
</ul>
