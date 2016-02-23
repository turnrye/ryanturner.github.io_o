---
layout: page
title: Hi, I'm Ryan.
tagline: I do web, mobile, and WiFi.
---
## What I do
I'm a mobile and web application developer from Memphis with experience in WiFi network engineering as well. I can whip up a killer app or site for you.

## Recent Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
