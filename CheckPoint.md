{% assign pp = site.pages | sort_natural: "title" %}
{% for p in pp %} [{{ p.date | date: %M:%S" }}]({{ p.url }}){% endfor %}
