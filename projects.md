---
layout: page
title: Selected Projects
---

**Quick Navigation Links**:<b />
[[Current Projects](#current-projects)] [[Completed Projects](#completed-projects)]

----

## Current Projects

{% for pub in site.data.project_list.current %}
**{{pub.name}}**<br />
{{pub.description}}<br />
{% if pub.link %}<i class="fa fa-fw fa-github"></i> [View on Github]({{pub.link}}){% endif %}

{% endfor %}

----

## Completed Projects

{% for pub in site.data.project_list.completed %}
**{{pub.name}}**<br />
{{pub.description}}<br />
{% if pub.link %}<i class="fa fa-fw fa-github"></i> [View on Github]({{pub.link}}){% endif %}

{% endfor %}
