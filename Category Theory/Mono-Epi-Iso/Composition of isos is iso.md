---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
---
For [[Category|Morphisms]] $A\overset{f}{\to}B\overset{g}{\to}C$ and $A\overset{f^{-1}}{\gets}B\overset{g^{-1}}{\gets}C$, then
- if $f$ and $g$ have [[Left-right inverse|Left inverses]] $f^{-1}$ and $g^{-1}$, then $gf:A\to C$ has a left inverse $f^{-1}g^{-1}$.
- if $f$ and $g$ have [[Left-right inverse|Right inverses]] $f^{-1}$ and $g^{-1}$, then $gf:A\to C$ has a right inverse $f^{-1}g^{-1}$.
- if $f$ and $g$ are [[Isomorphism|isomorphisms]] with inverses $f^{-1}$ and $g^{-1}$, then $gf:A\to C$ is an isomorphism with inverse $(gf)^{-1}=f^{-1}g^{-1}$.
##### Proof:
- Left inverses $\implies$ Composite has left inverse:
	$(f^{-1}g^{-1})(gf)=f^{-1}\big((g^{-1}g)f)=f^{-1}(\operatorname{id}_B f)= f^{-1}f=\operatorname{id}_A$, so $f^{-1}g^{-1}$ is left inverse of $gf$.
- Right inverses $\implies$ Composite has right inverse:
	$(gf)(f^{-1}g^{-1})=g\big((ff^{-1})g^{-1}\big)=g(\operatorname{id}_B g^{-1})=gg^{-1}=\operatorname{id}_C$, so $f^{-1}g^{-1}$ is right inverse of $gf$.
- Isomorphisms $\implies$ Composite is isomorphism:
	By the previous results $(gf)^{-1}=f^{-1}g^{-1}$ is the inverse of $gf$.