{% assign pp = site.pages | sort_natural: "info" %}
{% for p in pp %} [{% if p.info == "" %}{% if p.name == "" %}_{% else %}{{ p.name }}{% endif %}{% else %}{{ p.info }}{% endif %}]({{ p.url }}){% endfor %}
