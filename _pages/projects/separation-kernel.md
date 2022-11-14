---
title: Separation Kernel
permalink: /projects/separation-kernel/
members:
  - Henrik Karlsson
  - Roberto Guanciale
  - Mads Dam
---

A typical software system consists of thousands of complex components that are often designed with security as an afterthought. The result is bugs and security holes, some of which allow adversaries to gain complete control of a remote system. As shown by the Spectre and Meltdown vulnerabilities, the situation is similar in the hardware. It shouldn’t be like this, and it doesn’t have to.

<iframe  src="https://www.youtube.com/embed/sGE8CeWeMGE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

To improve on this situation, we need to build systems in new ways using rigorous techniques known as formal methods. Formal methods allow us to prove, using mathematics and logic, the absence of vulnerabilities and bugs. In other words, formal methods can allow us to build virtually unbreakable and unhackable systems.

Formal methods have, however, been known to be heavy-duty and require the software to be slim and specialized. But what is truly remarkable is that these techniques have recently been used in practice to verify the security real systems running on real hardware. These techniques have mainly been used to prove the security of systems on a software level, further research is required to extend these techniques to encompass the hardware.

In this project, we are developing new efficient methods, that allow us to verify both the software and the hardware. Our goal is to develop techniques good enough for the full-stack verification of a multicore real-time operating system for [RISC-V](https://en.wikipedia.org/wiki/RISC-V) that isolates critical software components from malfunctions in applications.

This project is funded by the [Center for Cyber Defence and Information Security (CDIS)](https://www.kth.se/cdis) at KTH.

---

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}

<div style="clear:both;"></div>

<h2>Resources</h2>
- [Simple Secure Separation Kernel (S3K) GitHub repository](https://github.com/kth-step/separation-kernel)
- [OpenMZ (Open MultiZone) Github reposititory](https://github.com/castor-software/openmz)
- [Poster (CDIS Spring Conference, 24 May 2022)](/assets/projects/separation-kernel/2022-cdis-poster.pdf)
- [CDIS Fall Retreat Slides (27 October, 2022)](/assets/projects/separation-kernel/2022-10-27-cdis-retreat.pdf)
- [30% Seminar Slides (8 November, 2022)](/assets/projects/separation-kernel/2022-11-08-seminar30.pdf)

