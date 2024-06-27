{% assign pp = site.pages | sort_natural: "title" %}
{% for p in pp %} [{{ p.title }}__]({{ p.url }}){% endfor %}
