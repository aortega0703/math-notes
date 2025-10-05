---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group isomorphism]]"
  - "[[Injectivity and surjectivity|Bijection]]"
---
A [[Group homomorphism]] $\phi: G -> H$ is a [[Group isomorphism]] if and only if it is a [[Injectivity and surjectivity|Bijection]].
##### Proof:
- Group isomorphism $ ==> $ Bijection:
	$\phi$ and $\phi^{-1}$ are also functions in $\mathbf{Set}$, so by [[Bijective iff isomorphism]] $\phi$ is a bijection.
- Bijection $ ==> $ Group isomorphism:
	If $\phi$ is also a function in $\mathbf{Set}$, so by [[Bijective iff isomorphism]] it has an inverse function $\phi^{-1}:H -> G$.
	- $\phi^{-1}$ is an homomorphism:
		Let $h_1,h_2 in H$, as $\phi$ is surjective then $h_1=\phi(g_1)$ and $h_2=\phi(g_2)$ for some $g_1,g_2 in G$. Then$$
		
			\phi^{-1}(h_1\cdot h_2)
			&= \phi^{-1}(\phi(g_1)\cdot\phi(g_2))\
			&= \phi^{-1}(\phi(g_1\cdot g_2))\
			&=g_1 \cdot g_2\
			&= \phi^{-1}(h_1)\cdot \phi^{-1}(g_2)
		
		$$Making $\phi^{-1}$ and homomorphism.
	Therefore $\phi$ is a group isomorphism.