---
title: Cryptographic Protocol Verification
permalink: /projects/crypto-protocol/
members:
  - Karl Norrman
---
Communication systems and protocols are often standardized to enable interoperability. Cryptographic protocols for key establishment, channel encryption and other tasks are part of these standards. Large and complex standards, such as those for mobile networks and internet protocols, include implicit requirements and frequently have vague security assumptions and goals. In this project we extract and formalize cryptographic protocols from 5G and IoT standards, define appropriate adversary models and security properties, and analyze the protocols in the symbolic model (using the Tamarin prover) as well as in the computational model (using traditional pen-and-paper proofs).

<h2>Researchers</h2>
{% assign mems = site.data.members.current | where_exp: "mem", "page.members contains mem.name " %}
{% include member_list.md members=mems %}
