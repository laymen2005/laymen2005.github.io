---
layout: page
title: "英语二笔记"
permalink: /english/
---

> 考研是一场孤独的修行，整理这些笔记是为了在砥砺前行的路上，留下一丝温情的痕迹。

<ul class="post-list">
  {% for post in site.categories.english %}
    <li style="margin-bottom: 20px; list-style: none; border-bottom: 1px dashed #e0dcd3; padding-bottom: 10px;">
      <span style="color: #999; font-size: 0.85em; display: block;">{{ post.date | date: "%Y-%m-%d" }}</span>
      <h3 style="margin: 5px 0;">
        <a href="{{ post.url | relative_url }}" style="color: #2c3e50; text-decoration: none;">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>
