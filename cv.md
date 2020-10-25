---
layout: resume
title: CV
---
## Current Occupation

Software Engineer (L1) at Twilio Czechia s.r.o, Prague, Czechia

## Education

`1990 - 1994`
__University Name__
Degree Awarded

`1995 - 1997`
__University Name__
Degree Awarded 

## Publications

<!-- A list is also available [online](https://scholar.google.co.uk/citations?user=LTOTl0YAAAAJ) -->

{% for pub in site.data.cv.publications %}
{{pub.author}}<br />
**{{pub.title}}**<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.month}}, {{pub.year}}*<br />
[[web]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})] {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}

{% endfor %}

## Theses

{% for pub in site.data.cv.theses %}
**{{pub.title}}**<br />
{{% if pub.type %}} {{pub.type}} {{% endif %}}*<br />
*{{pub.school}}* <br \>
*{{pub.address}}* {% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.month}}, {{pub.year}}* <br />
{% if pub.url %}[[View Thesis]({{pub.url}})]{% endif %}

{% endfor %}

## Occupation

`Nov 2020 - Present`
__Software Engineer (L1)__, Twilio Czechia s.r.o
Prague, Czechia  

`April - October 2020`
__Intern Software Engineer (L1)__, Twilio Czechia s.r.o 

- Task
- Task



<!-- ### Footer

Last updated: Oct 23, 2020 -->


