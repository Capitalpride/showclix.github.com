---
layout: page
title: Technically ShowClix
tagline: The ShowClix Blog for All Things Tech
---
{% include JB/setup %}

<div id="posts">
  {% for post in site.posts limit:5 %}
    <h1><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h1>
    <span>{{ post.date | date_to_string }}</span>
    <p>
    	{{post.content}}
    </p>
  {% endfor %}
</div>
