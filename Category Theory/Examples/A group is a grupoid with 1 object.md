---
tags:
  - theorem
  - category_theory
  - abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Grupoid]]"
  - "[[Category]]"
---
For a [[Grupoid]] $\mathcal{C}$ with a single [[Category|Object]] $*$, $(\text{Hom}_\mathcal{C}(*,*), \circ)$ is a [[Group]].
##### Proof:
- Closed:
	For any $f,g:*\to *$, $gf: *\to *$.
- Associative:
	For any $f,g,h:*\to *$, $(hg)f=h(gf)$ by definition of composition in a [[Category]].
- Has identity:
	For any $f:*\to *$, $f\text{id}_*=\text{id}_*f=f$ by definition of [[Category|Identity morphism]] in a [[Category]].
- Has inverses:
	For any $f:*\to *$ there exists some $f^{-1}:*\to *$ such that $ff^{-1}=f^{-1}f=\text{id}_*$ by definition of [[Grupoid]].