---
layout: default
title: Home
---

# posts!

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}"> <h2> {{ post.title }} </h2> </a>
        <p class="blogdate">{{ post.date | date: "%d %B %Y" }}</p>
        <div>{{ post.content |truncatehtml | truncatewords: 60 }}</div>
    </li>
  {% endfor %}
</ul>
