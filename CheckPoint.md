{% assign pp = site.pages | sort_natural: "title" %}
{% for p in pp %} [{{ site.time | date: %M:%S" }}]({{ p.url }}){% endfor %}
