---
title: Midterm Assignment
date: 2017-03-01
---

Submit solutions either using a proof assistant, or handwritten (or latexed). Note that solutions  must strictly follow the rules of homotopy type theory, with all terms constructed using such rules, except for inductive/recursive definitions which can be given in terms of cases, provided the cases correctly translate to use of `rec` and `induc` functions. __Do not__ use properties such as commutativity and associativity of addition - prove any lemmas you need starting with definitions in homotopy type theory.

A. Construct terms with the following types:
  1. $\\Pi_{A : \\mathcal{U}}\\Pi_{B: \\mathcal{U}} (A \\to (B \\to A))$.
  2. $\\Pi_{A : \\mathcal{U}}\\Pi_{B: \\mathcal{U}} (A \\to ((A \\to B) \\to B))$.

B. Recall the type $\\mathbf{2}$ is the type of Booleans, inductively defined by constructors $0 : \\mathbf{2}$ and $1 : \\mathbf{2}$, representing `false` and `true`, respectively.

1. Define the term $not : \\mathbf{2} \\to \\mathbf{2}$ representing the logical `not`.

2. Define the term $and: \\mathbf{2} \\to \\mathbf{2} \\to \\mathbf{2}$ representing the logical `and`.

3. Define the term $or: \\mathbf{2} \\to \\mathbf{2} \\to \\mathbf{2}$ representing the logical `or`.

4. Define the term $\\\_+\\\_ : \\mathbf{2} \\to \\mathbf{2} \\to \\mathbf{2}$ representing addition modulo $2$ (which is also the logical `xor`, i.e., exclusive or).

C. For the type $\\mathbf{2}$,

1. Construct a function $eq: \\mathbf{2} \\to \\mathbf{2} \\to \\mathbf{2}$ representing equality of terms (note that the final $\\mathbf{2}$ is to be viewed as booleans).

2. Construct a term of type $\\Pi_{a : \\mathbf{2}}\\Pi_{b: \\mathbf{2}}((a = b) \\to isTrue(eq(a)(b)))$.

3. Construct a term of type $\\Pi_{a : \\mathbf{2}}\\Pi_{b: \\mathbf{2}}(isTrue(eq(a)(b)) \\to (a = b))$.

D. The parity function from $\\mathbb{N}$ to $\\mathbf{2}$ maps even numbers to $0$ and odd numbers to $1$.

1. Define (in homotopy type theory) $parity: \\mathbb{N} \\to \\mathbf{2}$ which is as described above.

2. Construct a term of type (i.e., a proof of the proposition)  $\\Pi_{n : \\mathbb{N}}\\Pi_{m: \\mathbb{N}}(parity (n+m) = parity(n) + parity(m))$, where the first $\\\_+\\\_$ denotes the (recursively defined) addition on $\\mathbb{N}$ and the second denotes addition modulo $2$ on the type $\\mathbf{2}$ as defined above.

3. Consruct a function $half : \\mathbb{N} \\to \\mathbb{N}$ such that for any even number $2n$, $half(2n) = n$ (the values on odd numbers can be anything convenient).
