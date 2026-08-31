---
layout: default
---

Willkommen im offiziellen Wiki zum Pen&Paper-Setting **Kaltenstein**.

Baseurl: {{ site.baseurl }}

Justus Aurelius mit relative url: {{ "kaltenwiki/justus_aurelius_vk" | relative_url }}

Justus Aurelius ohne relative url: kaltenwiki/justus_aurelius_vk

Liste aller Artikel:

{% for x in site.kaltenwiki %}
* [{{ x.title }}]({{ x.url | relative_url }})
{% endfor %}
