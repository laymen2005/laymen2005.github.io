---
layout: page
title: "古文鉴赏"
permalink: /marks/
---

> “观古今之须臾，抚四海于一瞬。” 这里存放精选古文，每一篇都经过了细致的排版校对。

<ul class="post-list">
  {% for post in site.categories.marks %}
    <li style="margin-bottom: 20px; list-style: none; border-bottom: 1px dashed #e0dcd3; padding-bottom: 10px;">
      <span style="color: #999; font-size: 0.85em; display: block;">{{ post.date | date: "%Y年%m月%d日" }}</span>
      <h3 style="margin: 5px 0;">
        <a href="{{ post.url | relative_url }}" style="color: #8b4513; text-decoration: none;">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>
