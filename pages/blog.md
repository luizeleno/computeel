---
title: Blog
permalink: /blog/
mathjax: true
---

![blog]({{site.baseurl}}/assets/images/clipart/blog.jpg){: class="float-right rounded m-3 shadow-lg" width="30%"}

<div class="clearfix">

{% for post in site.categories.blog %}
<ul style="text-align: left">
<li>{{ post.date | date_to_long_string }}:
<a href="{{ post.url }}">{{ post.title | liquify }}</a></li>
</ul>
{% endfor %}

</div>
