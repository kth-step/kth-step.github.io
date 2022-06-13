---
title: Members
permalink: /members/
layout: single
---

{% include member_list.md members=site.data.members.current %}
<h2 style="clear:both;"> Collaborators </h2>
{% include member_list.md members=site.data.members.collaborators %}
<h2 style="clear:both;"> Past Members, Alumni and Collaborators </h2>
<ul style="list-style-type:none; padding-left:0;">
{% for mem in site.data.members.past %}
<li> {{ mem.name }}, {{ mem.position }}, {{ mem.affiliation }}{% if mem.date %}, ({{ mem.date }}){% endif %} </li>
{% endfor %}
</ul>
