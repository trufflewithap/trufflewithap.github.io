---
permalink: /media
layout: page
title: Media
---

{% for post in site.pages %}
{%- if post.permalink contains "media/" -%}
    <div style="margin-bottom: 30px;"><h1>{{ post.title }}</h1>
    <div class="media-scroll">
    {{ post.content }}
    </div></div>
{%- endif -%}  
{% endfor %}
