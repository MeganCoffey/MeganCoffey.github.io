---
layout: page
title: random
---


<div class="random">

  <ul class="posts">
    {% for post in site.categories.random %}

      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/about.md" | prepend: site.baseurl }}">via RSS</a></p>

</div>
