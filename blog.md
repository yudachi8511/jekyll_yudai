---
layout: default
title: Blog
---
<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url | relative_url }}">
	  {{ post.date | date: '%Y/%m/%d-%A' }} : {{ post.title }}
      </a></h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>