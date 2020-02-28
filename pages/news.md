---
layout: page
title: News
icon: <i class="far fa-newspaper"></i>
permalink: /news/
order: -1
---

<dl>
{% assign news = site.data.news | sort: 'date' | reverse %}
{% for n in news %}
<dt class="newslist-date">{{ n.date }}</dt>
<dd class="all">{{ n.news }}</dd>
{% endfor %}
