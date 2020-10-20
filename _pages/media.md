---
permalink: /media
layout: page
title: Media
---

{% for post in site.pages %}
{%- if post.permalink contains "media/" -%}
    <div style="padding-bottom: 20px;"><h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    <div style="max-height: 36vh; overflow-y: scroll; display: block;">
    {{ post.content }}
    </div></div>
{%- endif -%}  
{% endfor %}
