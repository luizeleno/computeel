---
layout: post
categories: news
title: "P. P. Ferreira, the newest MSci. at Computeel"
---

<div class="col-md-5 float-left mr-2">
{% include figure.html image='assets/images/defenses/mozao/mestrado/foto.png' modal=true id='defesa' caption="The official photo, pandemic-style" %}
</div>

Today the exam of our group member **[Pedro P. Ferreira]**, took place in our department. The work titled **"Ab initio investigation of superconducting and topological phases in transition metal dicalchogenides"** was supervised by **[Prof. Luiz T. F. Eleno]**.

Due to our current pandemic, the exam was carried out online via Google Meet.

Now the freshest Master of Science of the department, *Mozão* is about to start his PhD project working on state-of-the-art techniques in condensed matter. All the best!

<div class="w-100 mr-2">
<ul id="mestrado">
{% for foto in site.data.mozao.mestrado %}
<li data-thumb="{{site.baseurl}}/assets/images/defenses/mozao/mestrado/{{foto.foto}}"><img class="w-100" src="{{site.baseurl}}/assets/images/defenses/mozao/mestrado/{{foto.foto}}" /></li>
{% endfor %}
</ul>
</div>

<script type="text/javascript">
$(document).ready(function() {
    $('#mestrado').lightSlider({
        gallery: true,
        item: 1,
        loop: true,
        slideMargin: 0,
        thumbItem: 9
    });
});
</script>

[Pedro P. Ferreira]: {{site.baseurl}}/team/PiresPedro.html
[Prof. Luiz T. F. Eleno]: {{site.baseurl}}/team/01-luizeleno.html
