---
tags:
  - definition
  - math/category_theory
related topics:
  - "[[Category|Morphism]]"
reference:
  - Mac Lane, S. Categories for the Working Mathematician (1978)
aliases:
  - Epic
  - Monic
---
- A [[Category|Morphism]] $f: B -> C$ is monic (often $f: B \hookrightarrow C$) when for all $g,h: A -> B$$$
	f compose g= f compose h ==> g=h
$$
- A [[Category|Morphism]] $f: A -> B$ is epic (often $f: A \twoheadrightarrow B$) when for all $g,h: B -> C$, $$
	g compose f = h compose f ==> g=h
$$
Monomorphisms and Epimorphisms are [[Opposite category|Dual]] concepts.