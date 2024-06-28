{% assign pp = site.pages | sort_natural: "date" %}
{% for p in pp %} [{% if p.info == "" %}{% if p.name == "" %}{{ p.title }}{% else %}{{ p.name }}{% endif %}{% else %}{{ p.info }}{% endif %}{{ p.info }} __ ]({{ p.url }}){% endfor %}
