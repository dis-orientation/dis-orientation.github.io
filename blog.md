---
title: Dis-Orientation Collective Blog
layout: default-sidebar
---

## Dis-Orientation Collective Blog

{% for post in site.posts %}
{% if forloop.last != true %}
<div class="post">
<div class="preview-title">
<span class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
<br/>
<div class="date">{{ post.date | date: "%B %e, %Y" }}</div>
</div>
<div class="post-excerpt">
{{ post.content | split:"<!-- more -->" | first }}<br /><br />
<a href="{{ post.url }}">Read more ... </a><br />
</div>
</div>
{% else %}
<div class="post-last">
<div class="preview-title">
<span class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
<br/>
<div class="date">{{ post.date | date: "%B %e, %Y" }}</div>
</div>
<div class="post-excerpt">
{{ post.content | split:"<!-- more -->" | first }}<br /><br />
<a href="{{ post.url }}">Read more ... </a><br />
</div>
</div>
{% endif %}
{% endfor %}