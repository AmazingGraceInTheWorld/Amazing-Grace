
{% assign pp = site.pages | sort_natural: "info" %}

{% assign p.dd = "NO" %}

{% for p in pp %}
{% if p.info  %}{% assign d = p.info %}{% else %}{% if p.title %}{% assign d = p.title %}{% else %}{% assign d = p.name %}{% endif %}{% endif %}
{% assign p.dd = d %}
{% endfor %}

{% assign ppp = pp | sort_natural: "dd" %}

{% for p in ppp %} [{{ p.dd }}]({{ p.url }}){% endfor %}

Yes! 

Now {{ site.time | date: "%m-%d %H:%M:%S" }}


<!---{% if p.info  %}{{ p.info }}{% else %}{% if p.title %}{{ p.title }}{% else %}{{ p.name }}{% endif %}{% endif %} >


