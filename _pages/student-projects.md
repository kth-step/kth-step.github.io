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
    - if you know Standard ML or a similar language like OCaml, then you can write the implementation in this language, and discuss its correctness (pen-and-paper proof)
    - if you know HOL4 or some similar ITP, then you can do full proof of correctness in the ITP
      The translator may even be written in HOL4 itself, e.g. using existing parser generator `$HOLDIR/examples/formal-languages/context-free/pegScript.sml`
    - alternatively, building a translatior that translates Rust into the [Lem language](https://www.cl.cam.ac.uk/~pes20/lem/)
  - implementing a utility library for some of the primitive operations
  - testing the translated programs using test vectors by [Wycheproof](https://github.com/google/wycheproof) and NIST
  - validation of Rust against translated Standard ML implementation

  contact [Arve Gengelbach](https://www.kth.se/profile/arveg) and [Karl Palmskog](https://www.kth.se/profile/palmskog)

