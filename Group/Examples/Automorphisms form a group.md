---
tags:
  - theorem
  - category_theory
  - abstract_algebra
related topics:
  - "[[Automorphism]]"
  - "[[Group]]"
---
For a [[Category]] $\mathcal{C}$ and $A\in\operatorname{Obj}(\mathcal{C})$, $\operatorname{Aut}(A)$ is a [[Group]] under composition.
##### Proof:
- Closed:
	Let $f,g:A\overset{\sim}{\to} A$ be [[Automorphism|automorphisms]], then by [[Composition of isos is iso]] $gf:A\overset{\sim}{\to}A$ is an isomorphism, so $gf\in\operatorname{Aut}(A)$.
- Associative:
	By definition of [[Category]].
- Has identity:
	By [[Identity is iso]] $\operatorname{id}_A: A\overset{\sim}{\to}A$ is an isomorphism, so $\operatorname{id}_A\in\operatorname{Aut}(A)$. Let $f\in\operatorname{Aut}(A)$, then by unitality of [[Category|Identity morphism]] $\operatorname{id}_A f= f \operatorname{id}_A = f$, so $\operatorname{id}_A$ is an identity.
- Has inverses:
	Let $f\in\operatorname{Aut}(A)$, as $f:A\overset{\sim}{\to}A$ is an isomorphism there is some $f^{-1}:A\overset{\sim}{\to}A$ such that $ff^{-1}=f^{-1}f=\operatorname{id}_A$. By [[Inverse is iso]] $f^{-1}\in\operatorname{Aut}(A)$.
Therefore $\operatorname{Aut}(A)$ is a group.