---
title: HolBA Multicore
permalink: /projects/holba-mc/
members:
  - Didrik Lundberg
  - Henrik Karlsson
  - Pablo Buiras
  - Mads Dam
  - Roberto Guanciale
---

In this project we extend the HolBA with multicore semantics based on Promising RISC-V by Pulte et al.

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

<div style="clear:both;"></div>

<h2>Resources</h2>
- [HolBA Multicore](https://github.com/kth-step/HolBA-Multicore)
