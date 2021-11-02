---
layout: archive
permalink: /
title: 
---


<div class="front-cover" style="background:url(./images/{{ site.cover_image }}) no-repeat fixed center;background-size:cover;overflow:hidden;">
    
    <section>
        <div class="container" style="padding-top:1em;">
            <h1 style="text-align:center;color:#fff;font-weight:600;" id="site-title-front">{{ site.title }}</h1>
            {% if site.description %}<h3 style="text-align:center;color:#fff;font-weight:600;font-size:90%;">{{ site.description }}</h3>{% endif %}
        </div>
<div class="featured" style="border-top:1px solid grey;margin:0 10% 0 10%;">
<div style="background-image:linear-gradient(-130deg, rgba(14,21,58,0.3) 10%, rgba(74,76,123,0.5) 35%, rgba(161,140,171,0.2) 65%, rgba(243,201,215,0.2) 90%);">
{% for post in site.posts limit:1 %}
<h3 style="text-align:center;font-size:120%;">最新文章：<a href="{{ site.url }}{{ post.url }}" style="text-align:center;color:white;font-weight:600;">{{ post.title }}</a></h3>
<p style="text-align:left;color:#fff;font-size:90%;padding-bottom:0.5em;padding-left:2%;padding-right:2%;">{{ post.summary }}</p>
{% endfor %}
</div>
</div>
    </section>

</div>

欢迎来到黑河学院.麻了网，本站无任何官方背景，是在校学生出于好玩的目的而开发的。

目前已实装的功能有：

**(请点击相应项目进入简介）**

[麻了墙](https://hhxy.ml/projects/mlq/)

[麻了树洞](https://hhxy.ml/projects/treehole/)

[盲盒交友](https://hhxy.ml/projects/blindbox/)

如果你有什么好玩的想法，欢迎告诉我们！在论坛 [向管理员发送私信](http://q.hhxy.ml/member/admin) 、在 [微信公众号](https://i.loli.net/2021/11/02/Fd4MIkjWBUOxpSJ.jpg) 直接回复或向 [i@hhxy.ml](mailto:i@hhxy.ml)  发送邮件都可以联系到我们！

---

## 站务新闻

<div class="tiles">
{% for post in site.categories.news limit:5 %}
	{% include post-list-cn.html %}
{% endfor %}
</div><!-- /.tiles -->

	{% if site.categories.news.size %}
<a href="./news/">查看所有（共 {{ site.categories.news.size }} 篇）</a>
		{% else %}
暂无数据
		{% endif %}
