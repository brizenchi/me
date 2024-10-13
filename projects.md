---
layout: page
title: Projects
permalink: projects
---

<div>
  {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
  {% for post in sorted_projects %}
    <div class="py-1">
      <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.title}}</a></h3>
      <div class="text-sm text-gray-400">{{post.date | date: "%B %-d, %Y"}}</div>
    </div>
  {% endfor %}
</div>


