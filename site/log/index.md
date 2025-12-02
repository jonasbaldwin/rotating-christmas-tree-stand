---
layout: default
title: Progress Log
---

# Progress Log

Here's where I document my progress on building version 2 of the rotating Christmas tree stand.

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%B %d, %Y" }}</time></p>
      {% if post.excerpt %}
        <p>{{ post.excerpt }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
{% else %}
<p>No posts yet. Check back soon!</p>
{% endif %}

<style>
.post-list {
  list-style: none;
  margin-left: 0;
}
.post-list li {
  margin-bottom: 2em;
  padding-bottom: 1.5em;
  border-bottom: 1px solid #eee;
}
.post-list li:last-child {
  border-bottom: none;
}
.post-list h3 {
  margin-top: 0;
  margin-bottom: 0.5em;
}
.post-list time {
  color: #666;
  font-size: 0.9em;
}
</style>

