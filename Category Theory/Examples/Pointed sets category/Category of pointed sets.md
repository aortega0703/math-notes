---
tags:
  - definition
  - math/category_theory
related topics:
  - "[[Category]]"
  - "[[Category of sets]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
The [[Coslice category]] $\{*\}/\mathbf{Set}$ (with $\{*\}$ an arbitrary singleton) is denoted by $\mathbf{Set}^*$.
- Objects:
	For $f in\operatorname{arr}(\mathbf{Set})$$$
		f  in \operatorname{obj}(\mathbf{Set}^*)  <==> \operatorname{Dom}(f) = \{*\}
	$$These objects are _Pointed sets_ as the information in $f:\{*\}\to A$ is its codomain $S$ and a special element $f(*) in S$. Elements in $\mathbf{Set}^*$ are thus denoted $(s, S)$ with $S$ a set and $s in S$.
- Morphisms: 
	For $f: A\to B$ in $\mathbf{Set}$$$
	f  in \operatorname{Hom}_{\mathbf{Set}^*}((a, A),\ (b, B))  <==> f(a) = b
	$$
- Composition as usual.