---
title: HolBA
permalink: /projects/holba/
members:
  - Didrik Lundberg
  - Andreas Lindner
---

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

<div style="clear:both;"></div>

<h2>Resources</h2>
- [HolBA](https://github.com/kth-step/HolBA)
