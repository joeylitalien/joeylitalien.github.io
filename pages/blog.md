---
layout: page
title: Blog
icon: <i class="fas fa-rss-square"></i>
permalink: /blog/
order: -1
---

<div class="home">

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}  /
          {% for category in post.category %}
            <a href="{{category}}">{{category}}</a>
          {% endfor %}
        </span>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
