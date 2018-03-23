---
layout: blog
title: Blog
permalink: /blog/
---
<div class="small">以前のブログ「<a href="http://serialforeigner.com/">Serial Foreigner</a>」から、こちらに移行しました。（2018年3月）</div>
<div class="blog-list-font">
<ul>
  {% for post in site.categories.blog %}
<li class="home-list">
	<a href="{{ post.url }}" class="blog-link">{{ post.title }}</a>
	<span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
  <div class="blog-excerpt">{{ post.description }}</div>
</li>
{% endfor %}
</ul>
</div>
