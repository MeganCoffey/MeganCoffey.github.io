---
layout: channel
title: Data
permalink: /data/
---

<div class="data">

  <h1>data</h1>

  <ul class="posts">
    {% for post in site.posts %}

      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/about.md" | prepend: site.baseurl }}">via RSS</a></p>

</div>
