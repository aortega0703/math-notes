---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
---
For [[Category|Morphisms]] $A\overset{f}{ -> }B\overset{g}{ -> }C$ and $A\overset{f^{-1}}{\gets}B\overset{g^{-1}}{\gets}C$, then
- if $f$ and $g$ have [[Left-right inverse|Left inverses]] $f^{-1}$ and $g^{-1}$, then $gf:A -> C$ has a left inverse $f^{-1}g^{-1}$.
- if $f$ and $g$ have [[Left-right inverse|Right inverses]] $f^{-1}$ and $g^{-1}$, then $gf:A -> C$ has a right inverse $f^{-1}g^{-1}$.
- if $f$ and $g$ are [[Isomorphism|isomorphisms]] with inverses $f^{-1}$ and $g^{-1}$, then $gf:A -> C$ is an isomorphism with inverse $(gf)^{-1}=f^{-1}g^{-1}$.
##### Proof:
- Left inverses $ ==> $ Composite has left inverse:
	$(f^{-1}g^{-1})(gf)=f^{-1}\big((g^{-1}g)f)=f^{-1}(op("id")_B f)= f^{-1}f=op("id")_A$, so $f^{-1}g^{-1}$ is left inverse of $gf$.
- Right inverses $ ==> $ Composite has right inverse:
	$(gf)(f^{-1}g^{-1})=g\big((ff^{-1})g^{-1}\big)=g(op("id")_B g^{-1})=gg^{-1}=op("id")_C$, so $f^{-1}g^{-1}$ is right inverse of $gf$.
- Isomorphisms $ ==> $ Composite is isomorphism:
	By the previous results $(gf)^{-1}=f^{-1}g^{-1}$ is the inverse of $gf$.