{% assign pp = site.pages | sort_natural: "info" %}
{% for p in pp %} [{% if p.info == "" %}{% if p.title == "" %}A{% else %}{{ p.title }}BB{% endif %}{% else %}{{ p.info }}{% endif %}]({{ p.url }}){% endfor %}

Yes! 

Now {{ site.time | date: "%m-%d %H:%M:%S" }}
