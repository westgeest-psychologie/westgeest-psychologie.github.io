---
layout: page
title: Tarieven
permalink: /tarieven/
description: Onze tarieven voor psychologische consulten coaching en relatietherapie
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
Meld je je later af, dan wordt het volledige tarief in rekening gebracht.
Valt die 24 uur in het weekend? Stuur dan uiterlijk 24 uur van tevoren een mail of SMS met je afzegging of spreek mijn voicemail in.   


