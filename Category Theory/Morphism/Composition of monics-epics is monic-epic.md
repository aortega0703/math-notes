---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Monomorphism]]"
---
- For [[Monic-epic|Monics]] $A \overset{f}{\hookrightarrow} B \overset{g}{\hookrightarrow} C$, $g\circ f: A\hookrightarrow C$ is also monic.
- For [[Monic-epic|Epics]] $A \overset{f}{\twoheadrightarrow} B \overset{g}{\twoheadrightarrow} C$ , $g\circ f: A\twoheadrightarrow C$ is also epic.
##### Proof:
- $f,g$ monic $\implies$ $g\circ f$ monic:
	Let $h, h': S \to A$ such that $(g\circ f) \circ h = (g\circ f) \circ h'$, then$$
	\begin{align}
		g\circ f \circ h &= g\circ f \circ h'\\
		f \circ h &= f \circ h'
			&\text{by $g$ monic}\\
		h &= h'
			&\text{by $f$ monic}
	\end{align}
$$So $(g\circ f) \circ h = (g\circ f) \circ h' \implies h = h'$.
- $f,g$ epic $\implies$ $g\circ f$ epic:
	Let $h, h': C \to D$ such that $h \circ (g\circ f) = h'\circ (g\circ f)$, then$$
	\begin{align}
		h\circ g\circ f &= h\circ g\circ f\\
		h\circ g &= h\circ g
			&\text{by $f$ epic}\\
		h &= h'
			&\text{by $g$ epic}
	\end{align}
$$So $h\circ (g\circ f) = h'\circ (g\circ f) \implies h = h'$.