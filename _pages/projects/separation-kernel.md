---
title: Separation Kernel
permalink: /projects/separation-kernel/
---

A typical software system consists of thousands of complex components that are often designed with security as an afterthought. The result is bugs and security holes, some of which allow adversaries to gain complete control of a remote system. As shown by the Spectre and Meltdown vulnerabilities, the situation is similar in the hardware. It shouldn’t be like this, and it doesn’t have to.

To improve on this situation, we need to build systems in new ways using rigorous techniques known as formal methods. Formal methods allow us to prove, using mathematics and logic, the absence of vulnerabilities and bugs. In other words, formal methods can allow us to build virtually unbreakable and unhackable systems.

Formal methods have, however, been known to be heavy-duty and require the software to be slim and specialized. But what is truly remarkable is that these techniques have recently been used in practice to verify the security real systems running on real hardware. These techniques have mainly been used to prove the security of systems on a software level, further research is required to extend these techniques to encompass the hardware.

In this project, we are developing new efficient methods, that allow us to verify both the software and the hardware. Our goal is to develop techniques good enough for the full-stack verification of a multicore real-time operating system for RISC-V that isolates critical software components from malfunctions in applications.

<h2>Project members</h2>
<article>
<img src="https://www.kth.se/files/avatar/henrik10"/>
<h3>Henrik Karlsson</h3>
<p>PhD Student</p>
</article>
