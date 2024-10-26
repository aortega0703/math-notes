---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Equivalence relation]]"
  - "[[Injectivity and surjectivity|Bijectivity]]"
---
For a [[Set]] of sets $S$, a [[Relation]] $\cong$ defined on $S$ by$$
A\cong B\ \text{if and only if $A$ and $B$ are isomorphic}
$$is an [[Equivalence relation]].
##### Proof:
- Reflexivity:
	The identity function $\operatorname{id}_A:A\to A$ is clearly bijective, so $A\cong A$.
- Commutativity:
	Let $A\cong B$ (there is some $f:A\overset{\sim}{\to}B$ bijective), by [[Bijective iff inverse]] there is some $f^{-1}:B\overset{\sim}{\to}A$ and by [[Inverse of bijection is bijection]] it is also bijective, so $B\cong A$.
- Transitivity:
	Let $A\cong B$ and $B\cong C$ (there is some $f:A\overset{\sim}{\to}B$ and some $g:B\overset{\sim}{\to}C$ bijective), by [[Composition of injectives-surjectives is injective-surjective]] $g\circ f: A\overset{\sim}{\to}C$ is also bijective so $A\cong C$.
Therefore $\cong$ is an equivalence relation.