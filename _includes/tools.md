{% assign tools=site.tools | where:"type", "tool" | where:"cat", include.cat | where:"lang", page.lang | sort:"sort" %}
{% for tool in tools %}
{% include tool.md stable_version=tool.stable_version dev_version=tool.dev_version description=tool.description stable_status=tool.stable_status dev_status=tool.dev_status img=tool.img link=tool.permalink %}
{% endfor %}

