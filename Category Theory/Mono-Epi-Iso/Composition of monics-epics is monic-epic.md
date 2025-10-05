---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Monic-epic]]"
---
- For [[Monic-epic|Monics]] $A \overset{f}{\hookrightarrow} B \overset{g}{\hookrightarrow} C$, $g\circ f: A\hookrightarrow C$ is also monic.
- For [[Monic-epic|Epics]] $A \overset{f}{\twoheadrightarrow} B \overset{g}{\twoheadrightarrow} C$ , $g\circ f: A\twoheadrightarrow C$ is also epic.
##### Proof:
- $f,g$ monic $ ==> $ $g\circ f$ monic:
	Let $h, h': S -> A$ such that $(g\circ f) \circ h = (g\circ f) \circ h'$, then$$
	
		g\circ f \circ h &= g\circ f \circ h'\
		f \circ h &= f \circ h'
			&\text{by $g$ monic}\
		h &= h'
			&\text{by $f$ monic}
	
$$So $(g\circ f) \circ h = (g\circ f) \circ h' ==> h = h'$.
- $f,g$ epic $ ==> $ $g\circ f$ epic:
	Let $h, h': C -> D$ such that $h \circ (g\circ f) = h'\circ (g\circ f)$, then$$
	
		h\circ g\circ f &= h\circ g\circ f\
		h\circ g &= h\circ g
			&\text{by $f$ epic}\
		h &= h'
			&\text{by $g$ epic}
	
$$So $h\circ (g\circ f) = h'\circ (g\circ f) ==> h = h'$.