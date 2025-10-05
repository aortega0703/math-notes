---
tags:
  - theorem
  - definition
  - math/category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Dual
---
For a [[Category]] $\mathcal{C}$ its _opposite category_ $\mathcal{C}^{\operatorname{op}}$ is obtained by reversing all arrows. Spelled out this means it has
- Objects:
	$$A in \operatorname{obj}(\mathcal{C}^{\operatorname{op}}) <==> A in \operatorname{obj}(\mathcal{C})$$
	It has the same objects as $\mathcal{C}$.
- Morphisms:
	$$
	f in \operatorname{Hom}_{\mathcal{C}^\operatorname{op}}(B, A) <==> 
	f in \operatorname{Hom}_{\mathcal{C}}(A, B)
	$$
	It reverses arrow direction in $\mathcal{C}$.
- Composition:
	If $\circ$ is composition in $\mathcal{C}$ and $\circ^\operatorname{op}$ is composition in $\mathcal{C}^{op}$, then for $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $\mathcal{C}$.$$
		g\circ f = f\circ^\operatorname{op} g
	$$
Two definitions are _dual_ if one is obtained by reversing all arrows from the other.

---
$\mathcal{C}^\operatorname{op}$ is a category.
##### Proof:
- Identity:
	Consider $\operatorname{id}_A: A -> A$ in $\mathcal{C}$, by definition $\operatorname{id}_A: A -> A$ in $\mathcal{C}^\operatorname{op}$ too.
- Composition:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $C\overset{g}{ -> }B\overset{f}{ -> }A$ and $fg:C -> A$, so there exists some $gf:A -> C$ in $\mathcal{C}^\operatorname{op}$.
- Unitality:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $C\overset{g}{ -> }B\overset{f}{ -> }A$, $f\operatorname{id}_B = f$, and $\operatorname{id}_B g=g$. So in $\mathcal{C}^\operatorname{op}$ $\operatorname{id}_B f= f$ and $g\operatorname{id}_B =g$.
- Associative:
	Let $A\overset{f}{ -> }B\overset{g}{ -> }C\overset{h}{ -> }D$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $D\overset{h}{ -> }C\overset{g}{ -> }B\overset{f}{ -> }A$ and $(fg)h=f(gh)$. So in $\mathcal{C}^\operatorname{op}$ $(hg)f=h(gf)$.
Therefore $\mathcal{C}^\operatorname{op}$ is a category.