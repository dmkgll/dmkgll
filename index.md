---
layout: default
title: index
---

<style>ul {
    padding-inline-start: 0;
    list-style: none;
}</style>

<ul class="posts">
{% for post in site.posts %}
<li><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
 {% endfor %}</ul>
 
