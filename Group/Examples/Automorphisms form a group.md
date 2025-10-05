---
tags:
  - theorem
  - math/category_theory
  - math/abstract_algebra
related topics:
  - "[[Automorphism]]"
  - "[[Group]]"
---
For a [[Category]] $cal(C)$ and $A inop("Obj")(cal(C))$, $op("Aut")(A)$ is a [[Group]] under composition.
##### Proof:
- Closed:
	Let $f,g:A arrow.r.tilde A$ be [[Automorphism|automorphisms]], then by [[Composition of isos is iso]] $gf:A arrow.r.tilde A$ is an isomorphism, so $gf inop("Aut")(A)$.
- Associative:
	By definition of [[Category]].
- Has identity:
	By [[Identity is iso]] $op("id")_A: A arrow.r.tilde A$ is an isomorphism, so $op("id")_A inop("Aut")(A)$. Let $f inop("Aut")(A)$, then by unitality of [[Category|Identity morphism]] $op("id")_A f= f op("id")_A = f$, so $op("id")_A$ is an identity.
- Has inverses:
	Let $f inop("Aut")(A)$, as $f:A arrow.r.tilde A$ is an isomorphism there is some $f^{-1}:A arrow.r.tilde A$ such that $ff^{-1}=f^{-1}f=op("id")_A$. By [[Inverse is iso]] $f^{-1} inop("Aut")(A)$.
Therefore $op("Aut")(A)$ is a group.