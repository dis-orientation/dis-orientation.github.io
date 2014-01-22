---
title: Dis-orientation Collective Blog
layout: default
---

## `dis-orientation.info` Blog

{% for post in site.posts %}
{% if forloop.last != true %}
<div class="post">
<div class="preview-title">
<span class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
<br/>
<div class="date">{{ post.date | date: "%B %e, %Y" }}</div>
</div>
<div class="post-excerpt">
{{ post.content | split:"<!-- more -->" | first }}<br />
<a href="{{ post.url }}" class="excerpt-link">Read more ... </a><br />
<br/>
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
{{ post.content | split:"<!-- more -->" | first }}<br />
<a href="{{ post.url }}" class="excerpt-link">Read more ... </a><br />
<br/>
</div>
</div>
{% endif %}
{% endfor %}