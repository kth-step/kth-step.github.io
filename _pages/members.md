---
title: Members
permalink: /members/
layout: single
---

{% assign senior=site.data.members.current | where_exp:"m", "m.position != 'PhD student'" %}
{% assign phdstudents=site.data.members.current | where: "position", "PhD student" %}

{% include member_list.md members=senior %}
<h2 style="clear:both;">PhD Students</h2>
{% include member_list.md members=phdstudents %}

<h2 style="clear:both;"> Collaborators </h2>
{% include member_list.md members=site.data.members.collaborators %}

<h2 style="clear:both;">Former Members</h2>
{% include member_list.md members=site.data.members.past %}
