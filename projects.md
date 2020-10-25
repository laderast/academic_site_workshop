Jump to: [[Current Projects](#current-projects)] [[Completed Projects](#completed-projects)]

----

## Current Projects

{% for pub in site.data.project_list.current %}
**{{pub.name}}**<br />
{{pub.description}}<br />
{% if pub.link %}<a href={{ pub.link }}><i class="fa fa-fw fa-github"></i> View on Github</a>{% endif %}

{% endfor %}

## Completed Projects

{% for pub in site.data.project_list.completed %}
**{{pub.name}}**<br />
{{pub.description}}<br />
{% if pub.link %}<a href={{ pub.link }}><i class="fa fa-fw fa-github"></i> View on Github</a>{% endif %}

{% endfor %}
