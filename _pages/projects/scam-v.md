---
title: "SCAM-V: Side-Channel Abstract Model Validation"
permalink: /projects/scam-v/
members:
  - Pablo Buiras
  - Andreas Lindner
  - Roberto Guanciale
  - Hamed Nemati
  - Tiziano Marinaro
---
Observational models make tractable the analysis of information flow properties by providing an abstraction of side channels. Scam-V, Side-channel abstract model validation, is a tool for the validation of observational models for modern computer architectures. We combine symbolic execution, relational analysis, and different program generation techniques to generate experiments and validate the side-channel models. Validation of models is done by checking indistinguishability of the two inputs on real hardware by executing the program and analyzing the side channel. 

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

