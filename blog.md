---
layout: page
title: swirl | Blog
active: blog
---

<h1>The <img src="/images/swirl_new_large_final.png" height="50px" style="padding-bottom:10px"> Blog</h1>

{% assign posts = site.blog | sort: 'date' %}
{% for post in posts reversed %}
<li class="hidden-xs"><h3><a href="{{ post.url }}">{{ post.title }}</a>	
<span class="hidden-xs" style="width: 8em; float: right; ">{{ post.date | date: "%B %-d, %Y" }}</span></h3></li>

<li class="visible-xs text-center"><h3><a href="{{ post.url }}">{{ post.title }}</a></h3></li>
{% endfor %}
