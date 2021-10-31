---
layout: archive
title: 学校公告
---






{% if site.categories.history.size %}
共有 {{ site.categories.history.size }} 篇公告
		{% else %}
暂无公告
		{% endif %}

<div class="tiles">
{% for post in site.categories.history %}
	{% include post-list-cn.html %}
{% endfor %}
</div><!-- /.tiles -->
