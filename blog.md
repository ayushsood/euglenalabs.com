---
layout: page
title: Blog
permalink: /blog/
---
<ul class="post-list">
  {% for post in site.posts %}
      <li class="full-width">
        <a class="title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <div class="date">{{ post.date | date: "%b %-d, %Y" }}</div>

        <img src="{{ post.image }}" alt="blog image" />
        <div class="summary">{{ post.summary }} <a href="{{ post.url | prepend: site.baseurl }}">[Read More...]</a></div>
      </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

