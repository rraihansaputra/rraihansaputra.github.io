{% assign sorted = site.pages | sort: 'date' %}
{% for page in sorted %}
<h3><a title="{{ page.title }}" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></h3>
{% endfor %}   
Last update: {{ site.time | date_to_rfc822 }}

