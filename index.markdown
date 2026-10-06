---
layout: default
---

{% assign articles = site.kaltenwiki | sort: "title" %}
{% assign people = site.kaltenwiki | where: "person", "true" | sort: "name" %}

Willkommen im offiziellen Wiki zum Pen&Paper-Setting **Kaltenstein**.

Personen:

<ul>
{% for x in people %}
<li> <a href="{{ x.url | relative_url }}">{{ x.title }}</a> </li>
{% endfor %}
</ul>

Institutionen:

<ul>
{% for x in articles %}
{% if x.institution %}
<li> <a href="{{ x.url | relative_url }}">{{ x.title }}</a> </li>
{% endif %}
{% endfor %}
</ul>

Orte: 

<ul>
{% for x in articles %}
{% if x.place %}
<li> <a href="{{ x.url | relative_url }}">{{ x.title }}</a> </li>
{% endif %}
{% endfor %}
</ul>

Andere:

<ul>
{% for x in articles %}
{% unless x.person or x.institution or x.place %}
<li> <a href="{{ x.url | relative_url }}">{{ x.title }}</a> </li>
{% endunless %}
{% endfor %}
</ul>

Styleguide für Mitwirkende:
* **Fett** ist für Definitionen: Der Begriff, um den es auf der jeweiligen Seite geht; seine Synonyme/Aliase; Unterbegriffe, die auf dieser Seite eingeführt werden.
* *Kursiv* ist für Begriffe, die auf der jeweiligen Seite nicht definiert werden und auch nicht verlinkt sind. Nur die erste Nennung des Begriffes auf der Seite wird kursiv gesetzt. Werden Begriffe in einer Liste aufgezählt, kann auf Kursivsetzung verzichtet werden.
* Wann immer möglich (d.h. wenn eine entsprechende Seite existiert), soll zu verwendeten Begriffen ein [Link]({{ "/" | relative_url }}) gesetzt werden. Außer natürlich, wenn der Link wieder auf dieselbe Seite führt.
