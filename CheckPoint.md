{% assign pp = site.pages | sort_natural: "date" %}
{% for p in pp %} [{{ p.date }} __ ]({{ p.url }}){% endfor %}
