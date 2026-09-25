---
layout: default
title: Home
---

<h1>Latest posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>

      <time datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%d %B %Y" }}
      </time>
    </li>
  {% endfor %}
</ul>

