{% assign pp = site.pages | sort_natural: "date" %}
{% for p in pp %} [{{ p.date }}___]({{ p.url }}){% endfor %}
