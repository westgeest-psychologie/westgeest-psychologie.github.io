---
layout: page
title: Tarieven
---

<table>
<tr> <th>Type Sessie </th> <th>Duur van de Sessie</th><th>Tarief</th><th>Tarief buiten kantoortijden</th></tr>
{% for sessie in site.data.tarieven %}
<tr>
<td>{{ sessie.sessie_type }}</td>
<td>{{ sessie.duur }}</td>
<td>{{ sessie.tarief }}</td>
<td>{{ sessie.tarief_buiten_kantoortijden }}</td>
</tr>
{% endfor %}
</table>

## Afmelden

Mocht je een sessie moeten afmelden, doe dat dan ten minste 24 uur van tevoren. Zo kan ik nog een andere client inplannen. 
Meld je je later af, moet ik het "No-show" tarief in rekening brengen. 


