<ul style="list-style-type:none; padding-left:0;">
{% for pub in include.publications.publications %}
<li> 
{% if pub.url %}
<b><a href="{{ pub.url }}">{{ pub.title }}</a>.</b>
{% else %}
<b>{{ pub.title }}.</b> 
{% endif %}
{{ pub.authors }}. 
{{ pub.pub }}.
{{ pub.year }}. </li>
{% endfor %}
</ul>

<h2>Master's Thesis</h2>
<ul style="list-style-type:none; padding-left:0;">
{% for pub in include.publications.masters %}
<li> 
{% if pub.url %}
<b><a href="{{ pub.url }}">{{ pub.title }}</a>.</b>
{% else %}
<b>{{ pub.title }}.</b> 
{% endif %}
{{ pub.authors }}. 
{{ pub.year }}. </li>
{% endfor %}
</ul>
