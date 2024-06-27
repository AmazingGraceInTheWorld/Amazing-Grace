{% assign pp = site.pages | sort_natural: "date" %}
{% for p in pp %} [{{ p.date | date: %M:%S" }}]({{ p.url }}){% endfor %}
