---
layout: default
title: Jill
---

## Welcome to jillholmes.com

<ul class="post-list">
{% for post in site.posts limit:3 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-date">— {{ post.date | date: "%B %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>

<p>
  <a href="{{ '/updates' | relative_url }}">View all updates →</a>
</p>