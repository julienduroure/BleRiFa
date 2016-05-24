{{ page.description }}  
  
| Version | {{ page.version }} |
| status  | {{ page.description }} |
| | {% if page.display_url == true %}{% for url in page.getit_url %}{{ site.data.trad["getit"][page.lang] }} [{{url.label}}]({{ url.url}})<br/>{% endfor %} {% else %} *{{ site.data.trad["no_download"][page.lang] }}* {% endif %} |
{: class="tool_tab"}

