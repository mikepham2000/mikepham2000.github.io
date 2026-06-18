---
layout: page
title: Home
---

# Nguyen Phat Huy Pham

**Animal breeding & genetics • quantitative genetics • swine • disease resilience**

Hi! I'm a Ph.D. candidate in Animal Breeding and Genetics at [Iowa State University](https://www.iastate.edu/), working in the lab of [Dr. Jack C. M. Dekkers](https://www.ans.iastate.edu/people/jack-dekkers). My research uses quantitative and statistical genetics to improve livestock — currently focused on swine reproductive performance, carcass and meat quality, and the genetic signals of disease resilience.

A central thread of my work is genotype-by-environment interaction: understanding why an animal that excels on one farm may rank differently on another half a world away. My recent work compares North American and Southeast Asian herds, and explores gene co-expression networks in blood as potential indicators of disease resilience.

## Explore

- **[About](/about/)**: My background, education, and research
- **[Publications](/publications/)**: Peer-reviewed articles, manuscripts, and presentations
- **[Blog](/blog/)**: Notes on research, genetics, and tools
- **[CV]({{ site.cv_file | relative_url }})**: Download my full curriculum vitae (PDF)

## Recent Posts

<div class="post-list">
  {% for post in site.posts limit:3 %}
    <article class="post-preview">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
    </article>
  {% endfor %}
</div>

[View all posts →](/blog/)

## Get in Touch

- **Email**: [phamhuy2@iastate.edu](mailto:phamhuy2@iastate.edu)
- **GitHub**: [@mikepham2000](https://github.com/mikepham2000)

---

*This website is built with Jekyll and hosted on GitHub Pages.*
