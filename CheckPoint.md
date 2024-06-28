{% assign pp = site.pages | sort_natural: "info" %}
{% for p in pp %} [{% if p.info == "" %}AA{% else %}{{ p.info }}{% endif %}]({{ p.url }}){% endfor %}

Yes! 

Now {{ site.time | date: "%m-%d %H:%M:%S" }}
