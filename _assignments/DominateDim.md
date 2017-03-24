---
title: Domination and Levels
date: 2014-04-04
---

For types $X$ and $Y$, define
$Dominates(X)(Y):= \\sum\\limits\_{f: X \\to Y} \\sum\\limits\_{g: Y \\to X} f \\circ g \\sim id\_Y$. If a term of this type exists we say $X$ dominates $Y$.


1. Prove (i.e., construct a term of  type) $Dominates(X)(Y) \\to isPropn(X) \\to isPropn(Y)$.

2. Prove
$Dominates(X)(Y) \to \\prod\\limits\_{a, b: Y}\\sum\\limits\_{c, d: X} Dominates(c = d)(a = b)$.

3. Suppose $X$ dominates $Y$. Conclude that if $X$ has level at most $n$ (where $n \\geq -1$) then $Y$ has level at most $n$.
