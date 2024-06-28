{% assign pp = site.pages | sort_natural: "info" %}
{% for p in pp %} [{% if p.info  %}{{ p.info }}{% else %}{% if p.title %}{{ p.title }}{% else %}{{ p.name }}{% endif %}{% endif %}]({{ p.url }}){% endfor %}

Yes! 

Now {{ site.time | date: "%m-%d %H:%M:%S" }}
