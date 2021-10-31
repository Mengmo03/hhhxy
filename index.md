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

黑河学院（Heihe University），坐落于黑龙江省黑河市，是经教育部批准成立的一所普通高等本科院校，是中俄合作应用型人才培养创新实验区、国家级语言文字规范化示范校，是教育部第一批确定的“中俄联合培养本科生项目”单位、是黑龙江省特色应用型本科高校培育单位。

学校始建于1958年，历经黑河师范专科学校、齐齐哈尔大学黑河分校等发展阶段；2004年晋升为本科院校，更名为黑河学院；2017年获批新增硕士学位授权立项建设单位。

据2020年7月学校官网显示，学校占地面积61.53万平方米，校舍建筑面积24.44万平方米，固定资产总值4.56亿元；教学科研仪器设备值10732.95万元；设二级学院14个，开设39个本科专业；有教职工844人，其中专任教师584人；全日制在校生10747人。

---

## 最新新闻

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

## 疫情防控

<div class="tiles">

{% for post in site.categories.covid limit:5 %}
	{% include post-list-cn.html %}
{% endfor %}

</div><!-- /.tiles -->



	{% if site.categories.covid.size %}
<a href="./stories/">查看所有（共 {{ site.categories.covid.size }} 篇）</a>
		{% else %}
暂无数据
		{% endif %}


## 学校公告

<div class="tiles">
{% for post in site.categories.notice limit:5 %}
	{% include post-list-cn.html %}
{% endfor %}
</div><!-- /.tiles -->



{% if site.categories.notice.size %}
<a href="./history/">查看所有（共 {{ site.categories.notice.size }} 篇）</a>
		{% else %}
暂无数据
		{% endif %}

