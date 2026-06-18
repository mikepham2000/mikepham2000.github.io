---
layout: home
title: Home
---

# Welcome to My Website

Hi! I'm **Mike Pham**, a passionate software developer and tech enthusiast. This is my personal corner on the internet where I share my projects, write about technology, and showcase my work.

## About Me

I'm interested in building great software, exploring new technologies, and collaborating with talented people. On this site you'll find:

- **Blog Posts**: Articles about programming, development, and tech topics
- **Projects**: Showcases of my work and open-source contributions
- **Portfolio**: My professional background and skills

## Recent Posts

<div class="post-list">
  {% for post in site.posts limit:3 %}
    <article class="post-preview">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ post.url }}" class="read-more">Read more →</a>
    </article>
  {% endfor %}
</div>

[View all posts →](/blog/)

## Get in Touch

Feel free to reach out! You can find me on:

- **GitHub**: [@mikepham2000](https://github.com/mikepham2000)
- **Email**: contact@mikepham2000.com

---

*This website is built with Jekyll and hosted on GitHub Pages.*
