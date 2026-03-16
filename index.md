---
layout: default
---

<div class="main-columns">
  <div class="column">
    <h2 class="column-title">英语题</h2>
    <ul class="post-list">
      {% for post in site.categories.english %}
        <li>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title }}
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>

  <div class="column">
    <h2 class="column-title">古文鉴赏</h2>
    <ul class="post-list">
      {% for post in site.categories.marks %}
        <li>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title }}
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
  .main-columns {
    display: flex;
    justify-content: space-between;
    gap: 40px;
    margin-top: 30px;
  }
  .column {
    width: 48%;
  }
  .column-title {
    border-bottom: 2px solid #4a7c44;
    padding-bottom: 10px;
    margin-bottom: 20px !important;
    font-size: 24px !important;
  }
  .post-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .post-list li {
    margin-bottom: 15px;
    border-bottom: 1px solid #f0f0f0;
    padding-bottom: 8px;
  }
  
  /* 移动端自动变成上下排列 */
  @media (max-width: 768px) {
    .main-columns {
      flex-direction: column;
    }
    .column {
      width: 100%;
    }
  }
</style>