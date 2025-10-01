---
tags:
  - definition
  - theorem
  - category_theory
  - needs_source
related topics:
  - "[[Preorder]]"
---
A [[Preorder]] $\lesssim$ on $S$ induces a category (say $S_\lesssim$) defined by
- Objects:
	$$ s in \operatorname{Obj}(S_\lesssim)  <==> s in S$$
	its objects are the elements of $S$.
- Morphisms:
	$$(a,b) in\operatorname{Hom}_{S_\lesssim}(a,b)  <==> a\lesssim b$$
	there exists a single morphism from $a$ to $b$ when $a\lesssim b$, otherwise $\operatorname{Hom}_{S_\lesssim}(a,b)=\emptyset$.
- Composition:
	$$a\overset{(a,b)}{\to}b\overset{(b,c)}{\to}c \implies a\overset{(a,c)}{\to}c$$
---
$S_\lesssim$ is a category.
##### Proof:
- Identities:
	Let $a in \operatorname{Obj}(S_\lesssim)$, then $a in S$ and $a\lesssim a$, so $a\overset{(a,a)}{\to}a$.
- Composition:
	Let $a\overset{(a,b)}{\to}b\overset{(b,c)}{\to}c$, then $a\lesssim b \lesssim c$ so $a\lesssim c$. Therefore $a\overset{(a,c)}{\to}c$, so $(b,c)\circ(a,b)=(a,c)$.
- Unitality:
	Let $a\overset{(a,b)}{\to}b\overset{(b,c)}{\to}c$, then $(b,c)\circ(b,b)=(b,c)$ and $(b,b)\circ(a,b)=(a,b)$.
- Associativity:
	Let $a\overset{(a,b)}{\to}b\overset{(b,c)}{\to}c\overset{(c,d)}{\to}d$, then$$
	
		\big((c,d)\circ(b,c)\big)\circ(a,b)
		&=(b,d)\circ (a,b)\
		&=(a,d)\
		&=(c,d)\circ(a,c)\
		&=(c,d)\circ\big((b,c)\circ(a,b)\big)
	
	$$
So $S_\lesssim$ is a category.