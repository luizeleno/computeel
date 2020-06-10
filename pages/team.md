---
title: Team
permalink: /team/
mathjax: true
---

<a name="members">
# Members

<table class="table table-hover">
<col width="25%">
<col width="75%">
{% for membro in site.team %}
  {% if membro.staff == "member" %}
<tr>
<td><img class="shadow-lg rounded" src="{{site.baseurl}}/assets/images/people/{{membro.image}}.jpg" width="100%" align="left" ></td>
<td class="align-middle"><b><a href="{{membro.url}}">{{ membro.title  }}</a></b> <i>(aka {{ membro.apelido }})</i>
<br>{{ membro.position }}
{% if membro.present %}
<br><i>Present address: </i>{{ membro.present }}
{% endif %}
{% if membro.CV %}
<br>
<a href="{{site.baseurl}}/assets/CVs/{{membro.CV}}.pdf">CV (pdf)</a>
{% endif %}
</td>
</tr>
{% endif %}
{% endfor %}
</table>

<a name="theor">
---
# Theoretical Collaborators

<table class="table table-hover">
<col width="25%">
<col width="75%">
{% for membro in site.team %}
{% if membro.staff == "theoretical" %}
<tr>
<td><img class="shadow-lg rounded" src="/assets/images/people/{{membro.image}}.jpg" width="100%" align="left"></td>
<td class="align-middle"><b><a href="{{membro.url}}">{{ membro.title }}</a></b> <i>(aka {{ membro.apelido }})</i>
<br>{{ membro.position  }}
{% if membro.present %}
<br><i>Present address: </i>{{ membro.present }}
{% endif %}
</td>
</tr>
{% endif %}
{% endfor %}
</table>

<a name="exp">
---
# Experimental Collaborators

<table class="table table-hover">
<col width="25%">
<col width="75%">
{% for membro in site.team %}
  {% if membro.staff == "experimental" %}
<tr>
<td><img class="shadow-lg rounded" src="/assets/images/people/{{membro.image}}.jpg" width="100%" align="left"></td>
<td class="align-middle"><b><a href="{{membro.url}}">{{ membro.title  }}</a></b> <i>(aka {{ membro.apelido }})</i>
<br>{{ membro.position  }}</td>
</tr>
{% endif %}
{% endfor %}
</table>
