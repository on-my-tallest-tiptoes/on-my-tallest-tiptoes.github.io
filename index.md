---
layout: default
title: Home
---

dit is een test! - home page!

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        <h2> {{ post.title }} </h2>
        <p class="blogdate">{{ post.date | date: "%d %B %Y" }}</p>
        <div>{{ post.content |truncatehtml | truncatewords: 60 }}</div>
      </a>
    </li>
  {% endfor %}
</ul>
