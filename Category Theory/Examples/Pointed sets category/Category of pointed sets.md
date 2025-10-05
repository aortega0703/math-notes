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
	For $f inop("arr")(\mathbf{Set})$$$
		f in op("obj")(\mathbf{Set}^*) <==> op("Dom")(f) = \{*\}
	$$These objects are _Pointed sets_ as the information in $f:\{*\} -> A$ is its codomain $S$ and a special element $f(*) in S$. Elements in $\mathbf{Set}^*$ are thus denoted $(s, S)$ with $S$ a set and $s in S$.
- Morphisms: 
	For $f: A -> B$ in $\mathbf{Set}$$$
	f in op("Hom")_{\mathbf{Set}^*}((a, A),\ (b, B)) <==> f(a) = b
	$$
- Composition as usual.