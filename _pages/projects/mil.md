---
title: "Microarchitectural Modelling and Verification"
permalink: /projects/mil/
members:
  - Karl Palmskog
  - Ning Dong
  - Roberto Guanciale
  - Mads Dam
---
The Machine Independent Language (MIL) captures microarchitectural features such as out-of-order execution. MIL can be used as a form of abstract microcode language, e.g., as a target language for translating Instruction Set Architecture (ISA) instructions, and for reasoning about microarchitectural features that may cause unwanted information flows, e.g., side channels leaking secret information.

<ul>
<li><a href="https://zenodo.org/record/6997534">Machine Independent Language formalization and tools</a></li>
<li><a href="https://github.com/kth-step/mil">MIL GitHub Repository</a></li>
</ul>

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

