---
tags:
  - definition
  - math/linear_algebra
textbook: "[[Linear Algebra Done Right]]"
aliases:
  - Vector
---
A _vector space_ is a [[Set]] $V$ and a [[Field]] F with [[Binary Operation|Binary Operations]] $+: V times V -> V$ (addition) and $dot: F times V -> V$ (scalar multiplication) that has (for $u,v,w in V$ and $a,b in F$)
- Commutativity: $$u+v = v+u$$
- Associativity: $$
	
		(u + v) + w &= u + (v + w)\
		(a b)v &= a(b v)
	$$
- Distributivity: $$
	
		a(u+v) &= a u + a v\
		(a+b)v &= a v + b v
	$$
- Identities for $+,\cdot$: $$
 bold(0) in V quad s.t. quad bold(0)+v = v\
1v=v
$$
- Inverses for $+$: $$
	
		-v in V quad s.t. quad -v + v = 0\
		
	$$
# Notation
- Elements of a vector space are called _vectors_ or _points_.
- If $V$ and $F$ form a vector space, we say $V$ is a vector space _over_ $F$.
- A vector space over $RR$ is a _real vector space_.
- A vector space over $CC$ is a _complex vector space_.