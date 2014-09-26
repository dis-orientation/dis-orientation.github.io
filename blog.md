---
title: Dis-Orientation Collective Blog
layout: default-sidebar
---
<div id="blog-title-rule">
<h2 id="dis-orientation-collective-blog-title">DIS-ORIENTATION COLLECTIVE BLOG</h2>
</div>

{% for post in site.posts %}
<div class="post">
<img src="{{ site.url}}css/images/megaphonecircle.png" style="float:left; margin-right: 1em;" />
<span class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
<br />
<span class="date"><a href="{{ post.url }}">{{ post.date | date: "%B %e, %Y" }}</a></span>
</div>
{% endfor %}