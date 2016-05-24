{{ page.description }}  
  
| Stable Version | {{ page.stable_version }} |
| status  | {{ page.stable_status }} |
| Dev Version | {{ page.dev_version }} |
| status  | {{ page.dev_status }} |
| | {% if page.display_url == true %}{% for url in page.getit_url %}{{ site.data.trad["getit"][page.lang] }} [{{url.label}}]({{ url.url}})<br/>{% endfor %} {% else %} *{{ site.data.trad["no_download"][page.lang] }}* {% endif %} |
{: class="tool_tab"}

