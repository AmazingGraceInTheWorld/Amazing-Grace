
{% for p in site.pages %} {% if p.info  %}{% assign d = p.info %}{% else %}{% if p.title %}{% assign d = p.title %}{% else %}{% assign d = p.name %}{% endif %}{% endif %}[{{ d }},]({{ p.url }}){% endfor %}
