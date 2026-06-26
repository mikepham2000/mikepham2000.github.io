---
layout: default
permalink: /blog/
title: blog
nav: true
nav_order: 1
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3 # The number of links after the current page
---

<div class="post">
  <ul class="post-list">
    {% if page.pagination.enabled %}
      {% assign postlist = paginator.posts %}
    {% else %}
      {% assign postlist = site.posts %}
    {% endif %}

    {% for post in postlist %}
      {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
      {% assign year = post.date | date: '%Y' %}
      {% assign tags = post.tags | join: '' %}
      {% assign categories = post.categories | join: '' %}

      <li>
        {% if post.thumbnail %}
          <div class="row">
            <div class="col-sm-9">
        {% endif %}
        <h3>
          <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <p>{{ post.description }}</p>
        <p class="post-meta">{{ read_time }} min read &nbsp; &middot; &nbsp; {{ post.date | date: '%B %d, %Y' }}</p>
        <p class="post-tags">
          <a href="{{ year | prepend: '/blog/' | relative_url }}">
            <i class="fa-solid fa-calendar fa-sm"></i> {{ year }} </a>

          {% if tags != '' %}
            &nbsp; &middot; &nbsp;
            {% for tag in post.tags %}
              <a href="{{ tag | slugify | prepend: '/blog/tag/' | relative_url }}">
                <i class="fa-solid fa-hashtag fa-sm"></i> {{ tag }}</a>
              {% unless forloop.last %}
                &nbsp;
              {% endunless %}
            {% endfor %}
          {% endif %}

          {% if categories != '' %}
            &nbsp; &middot; &nbsp;
            {% for category in post.categories %}
              <a href="{{ category | slugify | prepend: '/blog/category/' | relative_url }}">
                <i class="fa-solid fa-tag fa-sm"></i> {{ category }}</a>
              {% unless forloop.last %}
                &nbsp;
              {% endunless %}
            {% endfor %}
          {% endif %}
        </p>
        {% if post.thumbnail %}
            </div>
            <div class="col-sm-3">
              <img class="card-img card-img-right" src="{{ post.thumbnail | relative_url }}" style="object-fit: cover; height: 90%; width: 100%" alt="post image">
            </div>
          </div>
        {% endif %}
      </li>
    {% endfor %}
  </ul>

  {% include pagination.liquid %}
</div>
