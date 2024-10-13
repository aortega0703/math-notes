---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Euclid's lemma]]"
  - "[[Divisibility]]"
  - "[[Divisibility|Prime]]"
---
If $p$ is prime and $p$ divides $a_1 a_2 \dots a_n$, then $p$ divides $a_i$ for some $i$.
##### Proof:
- Case $n=2$:
	By [[Euclid's lemma]].
- Case $n+1$:
	$p$ divides $a_1 a_2 \dots a_{n+1}=(a_1 a_2 \dots a_n)a_{n+1}$. By [[Euclid's lemma]] $p$ divides $a_1 a_2 \dots a_n$ or $a_{n+1}$. If $p$ divides $a_1 a_2 \dots a_n$ then by induction it divides $a_i$ for some $i\leq n$.
Therefore $p$ divides $a_i$ for some $i$.