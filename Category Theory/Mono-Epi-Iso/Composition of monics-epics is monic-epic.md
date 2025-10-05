---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Monic-epic]]"
---
- For [[Monic-epic|Monics]] $A \overset{f}{\hookrightarrow} B \overset{g}{\hookrightarrow} C$, $g compose f: A\hookrightarrow C$ is also monic.
- For [[Monic-epic|Epics]] $A \overset{f}{\twoheadrightarrow} B \overset{g}{\twoheadrightarrow} C$ , $g compose f: A\twoheadrightarrow C$ is also epic.
##### Proof:
- $f,g$ monic $ ==> $ $g compose f$ monic:
	Let $h, h': S -> A$ such that $(g compose f) compose h = (g compose f) compose h'$, then$$
	
		g compose f  compose h &= g compose f  compose h'\
		f compose h &= f compose h'
			&\text{by $g$ monic}\
		h &= h'
			&\text{by $f$ monic}
	
$$So $(g compose f) compose h = (g compose f) compose h' ==> h = h'$.
- $f,g$ epic $ ==> $ $g compose f$ epic:
	Let $h, h': C -> D$ such that $h compose (g compose f) = h' compose (g compose f)$, then$$
	
		h compose g compose f &= h compose g compose f\
		h compose g &= h compose g
			&\text{by $f$ epic}\
		h &= h'
			&\text{by $g$ epic}
	
$$So $h compose (g compose f) = h' compose (g compose f) ==> h = h'$.