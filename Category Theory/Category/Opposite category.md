---
tags:
  - theorem
  - definition
  - category_theory
related topics:
  - "[[Category]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Dual
---
For a [[Category]] $\mathcal{C}$ its _opposite category_ $\mathcal{C}^{\operatorname{op}}$ is obtained by reversing all arrows. Spelled out this means it has
- Objects:
	$$A\in \operatorname{obj}(\mathcal{C}^{\operatorname{op}}) \iff A\in \operatorname{obj}(\mathcal{C})$$
	It has the same objects as $\mathcal{C}$.
- Morphisms:
	$$
	f\in \operatorname{Hom}_{\mathcal{C}^\operatorname{op}}(B, A) \iff 
	f\in \operatorname{Hom}_{\mathcal{C}}(A, B)
	$$
	It reverses arrow direction in $\mathcal{C}$.
- Composition:
	If $\circ$ is composition in $\mathcal{C}$ and $\circ^\operatorname{op}$ is composition in $\mathcal{C}^{op}$, then for $A\overset{f}{\to}B\overset{g}{\to}C$ in $\mathcal{C}$.$$
		g\circ f = f\circ^\operatorname{op} g
	$$
Two definitions are _dual_ if one is obtained by reversing all arrows from the other.

---
$\mathcal{C}^\operatorname{op}$ is a category.
##### Proof:
- Identity:
	Consider $\operatorname{id}_A: A\to A$ in $\mathcal{C}$, by definition $\operatorname{id}_A: A\to A$ in $\mathcal{C}^\operatorname{op}$ too.
- Composition:
	Let $A\overset{f}{\to}B\overset{g}{\to}C$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $C\overset{g}{\to}B\overset{f}{\to}A$ and $fg:C \to A$, so there exists some $gf:A\to C$ in $\mathcal{C}^\operatorname{op}$.
- Unitality:
	Let $A\overset{f}{\to}B\overset{g}{\to}C$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $C\overset{g}{\to}B\overset{f}{\to}A$, $f\operatorname{id}_B = f$, and $\operatorname{id}_B g=g$. So in $\mathcal{C}^\operatorname{op}$ $\operatorname{id}_B f= f$ and $g\operatorname{id}_B =g$.
- Associative:
	Let $A\overset{f}{\to}B\overset{g}{\to}C\overset{h}{\to}D$ in $\mathcal{C}^\operatorname{op}$. Then in $\mathcal{C}$ we have $D\overset{h}{\to}C\overset{g}{\to}B\overset{f}{\to}A$ and $(fg)h=f(gh)$. So in $\mathcal{C}^\operatorname{op}$ $(hg)f=h(gf)$.
Therefore $\mathcal{C}^\operatorname{op}$ is a category.