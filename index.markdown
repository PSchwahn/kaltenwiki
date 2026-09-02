---
layout: default
---

Willkommen im offiziellen Wiki zum Pen&Paper-Setting **Kaltenstein**.

Liste aller Artikel:

<ul>
{% for x in site.kaltenwiki %}
<li> <a href="{{ x.url | relative_url }}">{{ x.title }}</a> </li>
{% endfor %}
</ul>

Styleguide für Mitwirkende:
* **Fett** ist für Definitionen: Der Begriff, um den es auf der jeweiligen Seite geht; seine Synonyme/Aliase; Unterbegriffe, die auf dieser Seite eingeführt werden.
* *Kursiv* ist für Begriffe, die auf der jeweiligen Seite nicht definiert werden und auch nicht verlinkt sind. Nur die erste Nennung des Begriffes auf der Seite wird kursiv gesetzt. Werden Begriffe in einer Liste aufgezählt, kann auf Kursivsetzung verzichtet werden.
* Wann immer möglich (d.h. wenn eine entsprechende Seite existiert), soll zu verwendeten Begriffen ein [Link]({{ "/" | relative_url }}) gesetzt werden. Außer natürlich, wenn der Link wieder auf dieselbe Seite führt.
