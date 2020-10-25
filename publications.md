---
layout: resume
title: List of Publications
---

[View on Google Scholar](https://scholar.google.co.uk/citations?user=aPd4T_YAAAAJ)

Jump to: [[Publications](#publications)] [[Theses](#theses)]

----

## Publications

{% for pub in site.data.cv.publications %}
`{{pub.year}}` 
{{pub.author}}<br />
**{{pub.title}}**<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})* {% endif %}<br />
[[web]({% if pub.internal %}{{pub.url | prepend: site.url}}{% else %}{{pub.url}}{% endif %})]
{% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}

{% endfor %}

----

## Theses

{% for pub in site.data.cv.theses %}
`{{pub.year}}`
**{{pub.title}}**<br />
{{% if pub.type %}} {{pub.type}}. Supervised by [{{pub.supervisor}}]({{pub.supervisor_link}})
{% if pub.supervisor2 %} and [{{pub.supervisor2}}]({{pub.supervisor2_link}}){% endif %}.{{% endif %}}<br />
*{{pub.school}}*<br />
In *{{pub.address}}* <br />
{% if pub.url %}[[View Thesis]({{pub.url}})]{% endif %}

{% endfor %}