---
title: News
permalink: /news/
mathjax: true
---

![news](/assets/images/clipart/news.png){: width="30%" class="float-right rounded m-3 shadow-lg"}

<div class="clearfix">

{% for post in site.categories.news %}
<ul style="text-align: left">
<li>{{ post.date | date_to_long_string }}:
<a href="{{ post.url }}">{{ post.title | liquify }}</a></li>
</ul>
{% endfor %}

</div>
