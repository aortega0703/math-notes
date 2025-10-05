---
tags:
  - theorem
  - math/abstract_algebra
  - math/category_theory
related topics:
  - "[[Category of abelian groups]]"
  - "[[Fiber product]]"
---
For [[Abelian group|Abelian groups]] $A,B$, their [[Fiber product]]$$
	A times_S B = \{(a,b)\ |\ \phi(a)=\psi(b),\ a in A,\ b in B\} subset.eq A times B
$$
with composition and projections from $A times B$ is also an Abelian group.
##### Proof:
![[fiber product.png]]
- $A times_S B$ is a [[Group]]:
	- Closed under $\cdot$:
		Let $(a,b),\ (a',b') in A times_S B$ so $(a,b)\cdot (a',b')=(aa',bb')$, then$$
		
			\phi(aa') 
			&= \phi(a)\phi(a')\
			&= \psi(b)\psi(b')\
			&= \psi(bb')
		
		$$
		Then $(aa',bb') in A times_S B$.
	- Associative:
		Inherited from $A times B$.
	- Identity:
		$\phi(e_A)=e_S=\psi(e_B)$ by [[Group homomorphisms preserve identity]], so $(e_A,e_B) in A times_S B$.
	- Inverses:
		Let $(a,b) in A times_S B$, then by [[Group homomorphism preserves inverses]]$$
		
			\phi(a^{-1})
			&= \phi(a)^{-1}\
			&= \psi(b)^{-1}\
			&= \psi(b^{-1})
		
		$$
		So $(a^{-1},b^{-1})=(a,b)^{-1} in A times_S B$.
	Then $A times_S B$ is a group.
- $A times_S B$ is [[Abelian group|Abelian]]:
	By [[Product of abelian groups is abelian]] $A times B$ is abelian, and $A times_S B subset.eq A times B$ so it is also Abelian.
Let$$

	f times g: X& -> A times_S B\
	x& |-> (f(x),g(x))

$$
 - $f times g$ is an [[Group homomorphism]]:
	 Let $x,x' in X$, then$$
	 
		 (f times g)(xx')
		 &= (f(xx'),\ g(xx'))\
		 &= (f(x)f(x'),\ g(x)g(x'))\
		 &= (f(x),\ g(x))\cdot(f(x'),\ g(x'))\
		 &= (f times g)(x)\cdot (f times g)(x')
	 
	 $$
	 Then $f times g: X -> A times_S B$ exists in $\mathbf{Ab}$.
- The diagram commutes:
	Let $x in X$, then$$
	
		(x)(f times g; \pi_1)
		&= (f(x),g(x))\pi_1\
		&= f(x)
	
	$$So by [[Set|Extensionality]] $(f times g; \pi_1) = f$. Similarly $(f times g; \pi_2)=g$.
- $f times g$ is unique:
	Let $x in X$ and $h,h':X -> A times_S B$ be homomorphisms such that the diagram commutes. Suppose $h(x)=(a,b)$ and $h'(x)=(a',b')$, then$$
	a=(a,b)\pi_1 = (x)(h\pi_1)=(x)f = (x)(h'\pi_1)= (a',b')\pi_1=a'
	$$Similarly$$
		b=(a,b)\pi_2 = (x)(h\pi_2)= (x)g = (x)(h'\pi_2)= (a',b')\pi_2=b'\
	$$So $h(x)=(a,b)=(a',b')=h'(x)$, and by [[Set|Extensionality]] $h=h'$, meaning $f times g$ is unique.
Then fiber products exists in $\mathbf{Ab}$.