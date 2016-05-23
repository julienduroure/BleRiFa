{% assign posts=site.posts | where:"type", "post" | where:"lang", page.lang %}{% for post in posts limit:3 %} | [{{post.title | truncate:30}}<br/>{% if post.img %}<img style="margin-top:10px;" src="{{ site.baseurl }}/assets/post/{{ post.img }}"/>{% endif %}]({{post.url}}) {%endfor%} |
{: class="resptable resp3"}
