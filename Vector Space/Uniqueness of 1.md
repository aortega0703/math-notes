---
tags:
  - theorem
  - math/linear_algebra
related topics:
  - "[[Vector Space]]"
  - "[[Field]]"
---
A [[Vector Space]] $V !=\{ bold(0)\}$ over $F$, has a unique identity for scalar multiplication.

##### Proof:
Let $v != bold(0) in V$, and suppose $1 != 1' in F$ be identities for scalar multiplication in $V$, then
$$

	1v 
		&= v\
		&= 1'v\
	1v - 1'v
		&= bold(0)\
	(1-1')v &= bold(0)\
	(1-1')^{-1} (1-1') v &= bold(0) \tag{1}\
	1v = bold(0)\
	v = bold(0)

$$
which is a contradiction as $v != bold(0)$ , so $1=1'$ making $1$ unique.
[^1]: by [[Uniqueness of additive inverse in Fields]] and [[Multiplication by 0 (vector)]].