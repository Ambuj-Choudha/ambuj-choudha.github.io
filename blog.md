---
layout: default
title: Blog
permalink: /blog/
---

# ~/blog

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <h3 class="post-item-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <div class="post-meta">
        {{ post.date | date: "%Y-%m-%d" }} :: {{ post.author | default: site.author }}
      </div>
      {% if post.tags %}
        <div class="tags">
          {% for tag in post.tags %}<span class="tag">#{{ tag }}</span>{% endfor %}
        </div>
      {% endif %}
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 220 }}</p>
      <a class="read-more" href="{{ post.url | relative_url }}">Read more</a>
    </li>
  {% endfor %}
</ul>
