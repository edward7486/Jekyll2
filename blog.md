---
title: Edward Nguyen's Blog
layout: blog
permalink: /blog/
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p class="post-date"> {{ post.date | date: '%B %d, %Y' }} </p>
      <p>{{ post.content | strip_html | truncatewords:60 }}</p>
    </li>
  {% endfor %}
</ul>