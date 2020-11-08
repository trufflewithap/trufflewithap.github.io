<!-- ---
permalink: /media
layout: page
title: Media
--- -->

# Media 

{% for post in site.pages %}
{%- if post.permalink contains "media/" -%}
    <div style="margin-bottom: 30px;"><h2>{{ post.title }}</h2>
    <div class="media-scroll">
    {{ post.content }}
    </div></div>
{%- endif -%}  
{% endfor %}
