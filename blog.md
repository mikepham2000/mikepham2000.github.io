---
layout: page
title: Blog
permalink: /blog/
---

# Blog

Welcome to my blog! Here I share notes on animal breeding and genetics, research, data analysis, and tools I find useful along the way.

<div class="post-list">
  {% if site.posts.size > 0 %}
    {% for post in site.posts %}
      <article class="post-preview">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
        <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span>
        {% if post.categories %}
          <div class="post-categories">
            {% for category in post.categories %}
              <span class="category-tag">{{ category }}</span>
            {% endfor %}
          </div>
        {% endif %}
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
      </article>
    {% endfor %}
  {% else %}
    <p>No posts yet. Check back soon!</p>
  {% endif %}
</div>
