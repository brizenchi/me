---
layout: page
title: Blog
permalink: blog
---

<div>
  {% assign blog = site.blog | sort: 'date' | reverse %}
  {% for post in blog %}
    <div class="py-1">
      <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.title}}</a></h3>
      <div class="text-sm text-gray-400">{{post.date | date: "%B %-d, %Y"}}</div>
    </div>
  {% endfor %}
</div>

