---
tags:
  - definition
  - set_theory
  - needs_source
related topics:
  - "[[Equivalence relation]]"
---
For a [[Function]] $f:A\to S$, the _kernel_ of $f$ is an [[Equivalence relation]] $\sim_f$ such that $a \sim_f b$ when $f(a) = f(b)$.
##### Proof:
- Reflexivity:
	Let $a\in A$, then $f(a)=f(a)$ so $a\sim_f a$.
- Commutativity:
	Let $a, b\in A$ such that $a\sim_f b$, then $f(a)=f(b)$ and $f(b)=f(a)$ so $b\sim_f a$.
- Transitivity:
	Let $a,b,c\in A$ such that $a\sim_f b$ and $b\sim_f c$, then $f(a)=f(b)$ and $f(b)=f(c)$ so $f(a)=f(c)$ and $a\sim_f c$.