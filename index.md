---
layout: home
title: dmkgll
---

<style>ul {
    padding-inline-start: 0;
    list-style: none;
}</style>

### Pages

- [Meta](/)
- [Mailing List](/)

### Latest updates

<ul class="posts">
{% for post in site.posts %}
<li><span>{{ post.date | date_to_string }}:</span> <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
 {% endfor %}</ul>
 
### Meta
 
 - Twitter: [@dmkgll](https://twitter.com/dmkgll)
 - GitHub: [@dmkgll](https://github.com/dmkgll)
 - Email: [dmkgll@protonmail.ch](/)
