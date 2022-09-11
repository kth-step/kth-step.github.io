---
title: Projects
permalink: /projects/
---

## The Trustfull project
{: #trustfull}

The Trustfull project is about trustworthy fullstack computing, i.e. it aims to show that formal techniques can be used in combination with static and dynamic manipulation techniques to strengthen security of real-life application stacks.

[Trustfull project's website](https://www.trustfull.proj.kth.se/){: .btn .btn--info}

## [HolBA - Formal Binary Analysis in HOL4](holba)
{: #holba}

HolBA is a platform for Binary Analysis in HOL4, a theorem prover.

[HolBA's GitHub repository](https://github.com/kth-step/holba){: .btn .btn--info}

### [Multicore](holba-mc)

In the HolBA Multicore project we extend the HolBA's BIR with the promising-semantics for multicore RISC-V.

## [Microarchitectural Modelling and Verification](mil)

[MIL GitHub repository](https://github.com/kth-step/mil){: .btn .btn--info}

## [Verified Pipelined Processor](pipeline-processor)

To improve the performance of processors, instruction pipelining is applied to handle multiple instructions concurrently by dividing instruction execution into different stages, like fetch and decode. Based on a verified Verilog model in the HOL4 interactive theorem prover, we implemented a typical 5-stage processor called Silver-Pi, for a simple instruction set architecture (ISA) Silver. This project is working on the correctness proof of the implementation with respect to the Silver ISA, and planning to analyse the information flow of programs on the circuit using the timing channel.

## CERCES/CERCES2, Pablo, Andreas

## [P4 Formalization](p4)

Software-Defined Networking (SDN) permits programming the data plane of the network devices using languages such as P4. This capability can impact network correctness due to error-prone programs. To address this, we have built a formalization of P4 semantics using the interactive theorem prover HOL4. This semantics allows us to analyse security properties in P4 packet forwarding programs.

## [SCAM-V](scam-v)

Observational models make tractable the analysis of information flow properties by providing an abstraction of side channels. Scam-V, Side-channel abstract model validation, is a tool for the validation of observational models for modern computer architectures. We combine symbolic execution, relational analysis, and different program generation techniques to generate experiments and validate the side-channel models. Validation of models is done by checking indistinguishability of the two inputs on real hardware by executing the program and analyzing the side channel. 

## [Cryptographic Protocol Verification](crypto-protocol)

## [Separation Kernel](separation-kernel)

In this project we design, implement and verify a separation kernel for high-assurance real-time systems running on RISC-V.

[Simple Secure Separation Kernel (S3K) GitHub repository](https://github.com/kth-step/separation-kernel){: .btn .btn--info}
[OpenMZ (Open MultiZone) Github reposititory](https://github.com/castor-software/openmz){: .btn .btn--info}
