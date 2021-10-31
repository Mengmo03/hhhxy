---
layout: archive
title: 学校公告
---






{% if site.categories.notice.size %}
共有 {{ site.categories.notice.size }} 篇公告
		{% else %}
暂无公告
		{% endif %}

<div class="tiles">
{% for post in site.categories.notice %}
	{% include post-list-cn.html %}
{% endfor %}
</div><!-- /.tiles -->
