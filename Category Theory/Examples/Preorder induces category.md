---
tags:
  - definition
  - theorem
  - math/category_theory
  - needs_source
related topics:
  - "[[Preorder]]"
---
A [[Preorder]] $\lesssim$ on $S$ induces a category (say $S_\lesssim$) defined by
- Objects:
	$$ s in op("Obj")(S_\lesssim) <==> s in S$$
	its objects are the elements of $S$.
- Morphisms:
	$$(a,b) inop("Hom")_{S_\lesssim}(a,b) <==> a\lesssim b$$
	there exists a single morphism from $a$ to $b$ when $a\lesssim b$, otherwise $op("Hom")_{S_\lesssim}(a,b)=\emptyset$.
- Composition:
	$$a\overset{(a,b)}{ -> }b\overset{(b,c)}{ -> }c ==> a\overset{(a,c)}{ -> }c$$
---
$S_\lesssim$ is a category.
##### Proof:
- Identities:
	Let $a in op("Obj")(S_\lesssim)$, then $a in S$ and $a\lesssim a$, so $a\overset{(a,a)}{ -> }a$.
- Composition:
	Let $a\overset{(a,b)}{ -> }b\overset{(b,c)}{ -> }c$, then $a\lesssim b \lesssim c$ so $a\lesssim c$. Therefore $a\overset{(a,c)}{ -> }c$, so $(b,c) compose (a,b)=(a,c)$.
- Unitality:
	Let $a\overset{(a,b)}{ -> }b\overset{(b,c)}{ -> }c$, then $(b,c) compose (b,b)=(b,c)$ and $(b,b) compose (a,b)=(a,b)$.
- Associativity:
	Let $a\overset{(a,b)}{ -> }b\overset{(b,c)}{ -> }c\overset{(c,d)}{ -> }d$, then$$
	
		\big((c,d) compose (b,c)\big) compose (a,b)
		&=(b,d) compose (a,b)\
		&=(a,d)\
		&=(c,d) compose (a,c)\
		&=(c,d) compose \big((b,c) compose (a,b)\big)
	
	$$
So $S_\lesssim$ is a category.