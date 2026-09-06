---
layout: default
title: 特依
---
---

欢迎！这里记录我的学习与思考。

--- 
## 文章列表

<ul>
{% for post in site.posts %}
<li>
<a href="{{ post.url }}">{{ post.title}}</a>
<span>· {{ post.date | date: "%Y-%m-%d" }}</span>
    <p>{{ post.excerpt}}</p>
    </li>
  {% endfor %}
</ul>

## 分类

<ul>
  {% for category in site.categories %}
    <li>
      <a href="/categories/{{ category[0] }}/">{{ category[0] }}</a>
      ({{ category[1].size }})
    </li>
  {% endfor %}
</ul>

## 标签

<ul>
  {% for tag in site.tags %}
    <li>
      <a href="/tags/{{ tag[0] }}/">{{ tag[0] }}</a>
      ({{ tag[1].size }})
    </li>
  {% endfor %}
</ul>

