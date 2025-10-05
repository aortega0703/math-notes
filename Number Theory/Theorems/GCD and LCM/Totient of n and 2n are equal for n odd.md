---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Group of units mod n]]"
  - "[[Euler's Phi Function|Euler's Totient Function]]"
---
For any odd $n > 0 in ZZ$, $\phi(2n) = \phi(n)$.
##### Proof:
- $\gcd(m, n) = 1 ==> \gcd(2m + n, 2n) = 1$:
	As $n$ is odd, then $2m+n$ is odd, so $\gcd(2m+n,2n)=\gcd(2m+n,n)$. By [[Relative Primes Iff Linear Combination Equals 1]] $am+bn=1$ for some $a,b in ZZ$. 
	- Rewriting of $xm+yn$:
		$$
		
			\frac{x}{2}(2m+n)+\left(y-\frac{x}{2}\right)n
			&= xm + \frac{xn}{2} + yn - \frac{xn}{2}\
			&= xm + yn
		
		$$
	- Case $a$ even:
		Let $x=a$ and $y=b$, then $\frac{a}{2}(2m+n)+\left(b-\frac{a}{2}\right)n=am+bn=1$, so $\gcd(2m+n, n)=1$.
	- Case $a$ odd:
		Let $x=a+n$ and $y=b-m$, then $\frac{x}{2}(2m+n)+\left(y-\frac{x}{2}\right)n=(a+n)m+(b-m)n=am+bn=1$, so $\gcd(2m+n, n)=1$.
	So $\gcd(m, n) = 1 ==> \gcd(2m + n, 2n) = 1$ for all $m,n$.
- $\gcd(r, 2n) = 1 ==> \gcd(\frac{r+n}{2} , n) = 1$:
	As $\gcd(r, 2n) = 1$ then $r$ is odd. By [[Relative Primes Iff Linear Combination Equals 1]] $ar+b2n=1$ for some $a,b in ZZ$. Consider$$
	
		2a\ \frac{r+n}{2} + (2b - a) n
		&= ar + an + b2n -an\
		&= ar + b2n\
		&= 1
	
	$$Then $\gcd(\frac{r+n}{2} , n) = 1$.
- $[m]_n \overset{f}{\mapsto} [2m + n]_{2n}$ is a bijection:
	- $f;\!f^{-1}=\text{id}_{\mathbb({Z}/n ZZ)^*}$:
		Let $m in\mathbb({Z}/n ZZ)^*$, then $(f;\!f^{-1})(m)\equiv f^{-1}(2m+n)\equiv\frac{2m+n+n}{2}\equiv m+n\equiv m\ (\text{mod }n)$.
	- $f^{-1};\!f=\text{id}_{\mathbb({Z}/2n ZZ)^*}$:
		Let $r in\mathbb({Z}/2n ZZ)^*$, then $(f^{-1};\!f)(r)\equiv f\left(\frac{r+n}{2}\right)\equiv 2\left(\frac{r+n}{2}\right)+n\equiv r+2n\equiv r\ (\text{mod }2n)$.
	Then by [[Bijective iff inverse]] $f$ is bijective.
This shows that $\mathbb({Z}/n ZZ)^*\cong\mathbb({Z}/2n ZZ)^*$ as sets, so their cardinality are equals, meaning $\phi(n)=\phi(2n)$ for $n>0$ odd.