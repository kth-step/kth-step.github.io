---
title: Verified Pipelined Processor
permalink: /projects/pipeline-processor/
members:
  - Ning Dong
---

To improve the performance of processors, instruction pipelining is applied to handle multiple instructions concurrently by dividing instruction execution into different stages, like fetch and decode. Based on a verified Verilog model in the HOL4 interactive theorem prover, we implemented a typical 5-stage processor called Silver-Pi, for a simple instruction set architecture (ISA) Silver. This project is working on the correctness proof of the implementation with respect to the Silver ISA, and planning to analyse the information flow of programs on the circuit using the timing channel.

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

