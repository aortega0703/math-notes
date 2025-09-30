---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group isomorphism]]"
  - "[[Order]]"
---
For any [[Group isomorphism]] $\phi: G\to H$ and $g\in G$,$$
\begin{align}
	|\phi(g)|=|g|
\end{align}
$$
##### Proof:
By definition $\phi$ has an inverse homomorphism $\phi^{-1}:H\to G$. By [[Group homomorphisms preserve order]] $|\phi(g)|$ divides $|g|$ and $|\phi^{-1}(\phi(g))|=|g|$ divides $|\phi(g)|$, so $|\phi(g)|=|g|$.