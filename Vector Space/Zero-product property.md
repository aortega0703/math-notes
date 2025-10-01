---
tags:
  - theorem
  - math/linear_algebra
related topics:
  - "[[Vector Space]]"
  - "[[Field]]"
---
In a [[Vector Space]] $V$ over $F$, $av= bold(0)$ implies $a=0$ or $v= bold(0)$ for all $v in V$ and $a in F$.
##### Proof:
By cases
- Case $a != 0$:$$
	
		av &=  bold(0)\
		a^{-1}av &=  bold(0)\tag{1}\
		v &=  bold(0)
	$$
[^1]: by [[Multiplication by 0 (vector)]].
- Case $v !=  bold(0)$:$$
	
		av &=  bold(0)\
		av + v &= v\
		av + 1v &= v\
		(a+1)v &= v\
		a+1 &= 1\tag{2}\
		a &= 0
	$$
[^2]: by [[Vector Space/Uniqueness of 1|Uniqueness of 1]].
Therefore either $a=0$ or $v= bold(0)$.