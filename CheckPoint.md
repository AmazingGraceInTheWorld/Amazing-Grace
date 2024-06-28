{% assign pp = site.pages | sort_natural: "date" %}
{% for p in pp %} [{{ p.info }} __ ]({{ p.url }}){% endfor %}
