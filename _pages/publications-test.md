---
title: "Publications Test"
permalink: /publications-test
layout: single
---
<ul id='publications' style="list-style-type:none; padding-left:0;">
</ul>
<script>
const step_authors = [{% for mem in site.data.members.current %} '{{mem.name}}', {% endfor %} 'R Guanciale', 'M Dam'];
const parser = new DOMParser();

fetch('assets/data/publications.rss')
.then(response => response.text())
.then(str => parser.parseFromString(str, "application/xml"))
.then(data => {
const items = data.querySelectorAll("item");
let html = ``;
items.forEach(el => {
let title = el.querySelector("title").innerHTML;
let url = el.querySelector("guid").innerHTML;
let authors = Array.from(el.querySelectorAll("creator")).map(x => x.innerHTML);
let date = new Date(el.querySelector("pubDate").innerHTML);
console.log(date);
const filteredArray = authors.filter(value => step_authors.includes(value));
if (filteredArray.length > 0) {
html += `<li><b><a href='${url}'>${title}</a></b>. ${authors.join(', ')}. ${date.getFullYear()}.</li>`;
}
});
document.getElementById('publications').innerHTML = html;
});
</script>

<h2>Master's Thesis</h2>
<ul style="list-style-type:none; padding-left:0;">
{% for pub in site.data.publications.masters %}
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
