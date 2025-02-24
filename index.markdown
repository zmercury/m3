---
layout: home
title: Welcome to My Blog
---

<div class="hero">
  <h1>Hey, I’m Mercury!</h1>
  <a href="/about" class="btn">Learn More About Me</a>
</div>

<section class="latest-posts">
  <h2>Latest Posts</h2>
  <ul>
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</section>
