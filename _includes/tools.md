{% assign tools=site.posts | where:"type", "tool" | where:"cat", include.cat | where:"lang", page.lang | sort:"sort" %}
{% for tool in tools %}
{% include tool.md version=tool.version description=tool.description status=tool.status img=tool.img link=tool.permalink getit=tool.getit_url %}
{% endfor %}

