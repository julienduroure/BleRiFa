{% assign tools=site.tools | where:"cat", include.cat | where:"lang", page.lang  %}
{% assign sorted_tools= tools | sort: 'sort_nb' %}
{% for tool in sorted_tools %}
{% include tool.md title=tool.title stable_version=tool.stable_version dev_version=tool.dev_version description=tool.description stable_status=tool.stable_status dev_status=tool.dev_status img=tool.img link=tool.permalink %}
{% endfor %}
