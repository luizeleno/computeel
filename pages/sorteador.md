---
title: Processo Seletivo - Edital ATAc/EEL/USP 10/2020
permalink: /sorteador/
layout: nosidebar
---

{% assign min = 1 %}
{% assign max = site.data.pontossorteio | size %}

## Pontos para a prova didática:

{% assign n=min%}
<ol>
{% for ponto in site.data.pontossorteio %}
<li><input id='{{n}}' class="form-control form-control-sm" type="text" placeholder="{{ponto}}"></li>
{% assign n=n | plus: 1%}
{% endfor %}
</ol>

---

<button type="button" id='sorteio' class='btn btn-primary' onclick="document.getElementById('pontosorteado').innerHTML = getRndInteger({{min}}, {{max}})">Sortear ponto</button>
<button type="button" class='btn btn-primary' onclick="resetstyle()">Reiniciar</button>

#### Ponto sorteado: <span class="badge badge-success" id="pontosorteado">&nbsp;&nbsp;</span>

<script>
function getRndInteger(min, max) {
  var num = Math.floor(Math.random() * (max - min + 1) ) + min;
  document.getElementById(num).style.fontWeight = "900";
  document.getElementById("sorteio").disabled = true;
  return num;
}
</script>

<script>
function resetstyle() {
  for(num={{min}}; num<={{max}}; num++) {
    document.getElementById(num).style.fontWeight = null;
    document.getElementById('pontosorteado').innerHTML = '&nbsp;&nbsp;';
    document.getElementById("sorteio").disabled = false;
  }
}
</script>
