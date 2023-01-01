---
layout: default
title: blog
---
<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts limit:4 %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
      <p>Posted by {{ post.author }}</p>
    </li>
  {% endfor %}
</ul>