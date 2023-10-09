---
title: Student Projects
permalink: /stud_projects/
---

There are various possibilities for thesis projects in the STEP group, which can be suitable for thesis projects depending on difficulty and scope.
Here we list some particular projects and contact details to members of the group.
The directions can be adjusted according to the interest of the student.


- Translating Rust Cryptography

  The [hacspec specification language for crypto](https://hacspec.org/) specifies cryptographic functions like AES-GCM 128 or Chacha20. Hacspec itself is a purely functional subset of the Rust language.
  The goal of this project is working towards being able to proving Rust code correct in a theorem prover, for which it needs to be translated into a different language.

  The suggested steps in the project are:

  - building a translator of a subset of Rust into (purely functional) Standard ML
    - if you know [Standard ML](https://smlfamily.org) or a similar language like [OCaml](https://ocaml.org), then you can write the implementation in this language, and discuss its correctness (pen-and-paper proof)
    - if you know [HOL4](https://hol-theorem-prover.org) or some similar Interactive Theorem Prover (ITP), then you can do full proof of correctness in the ITP
      The translator may even be written in HOL4 itself, e.g. using existing parser generator `$HOLDIR/examples/formal-languages/context-free/pegScript.sml`
    - alternatively, you can build a translator that translates Rust into the [Lem language](https://github.com/rems-project/lem), that can then be automtically exported to HOL4 or OCaml
  - implementing a utility library for some of the primitive operations
  - testing the translated programs using test vectors by [Wycheproof](https://github.com/google/wycheproof) and NIST
  - validation of Rust against translated Standard ML implementation

  contact [Arve Gengelbach](https://www.kth.se/profile/arveg) and [Karl Palmskog](https://www.kth.se/profile/palmskog)

- Fixing and extending a formally verified distributed key-value store

  A formally verified [distributed causally consistent key-value store](https://github.com/coq-community/chapar) was developed in the [Coq proof assistant](https://coq.inria.fr) and is now maintained on GitHub. While executable code can be extracted to OCaml and compiled together with library code to produce executable code, the key-value stores cannot be run due to issues in the OCaml library code. There are also several serious problems in the verified code, e.g., the formal specification assumes removal of duplicates while the OCaml implementation does not remove duplicates due to using the UDP protocol (see [issues](https://github.com/coq-community/chapar/issues) on GitHub).

  The suggested steps in the project are:

  - make the (extracted) OCaml code run again
  - fix the most serious issues such as message deduplication, at both the Coq and OCaml levels
  - practically evaluate the updated code on benchmark workloads

  contact [Karl Palmskog](https://www.kth.se/profile/palmskog)
