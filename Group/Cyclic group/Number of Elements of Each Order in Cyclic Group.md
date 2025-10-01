---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Cyclic group]]"
  - "[[Euler's Phi Function|Euler's Totient Function]]"
  - "[[Order]]"
---
For a cyclic group $\langle a \rangle$ and $d in ZZ$ a positive divisor of $|\langle a \rangle|$, the number of elements of $\langle a \rangle$ with order $d$ is $\varphi(d)$.
##### Proof:
By [[Fundamental Theorem of Cyclic Groups]] there is exactly one subgroup $\langle b\rangle lt.eq \langle a \rangle$ of order $d$. By [[Order of cyclic group is order of generator]] every element of order $d$ generates $\langle b \rangle$, and is therefore equal to $b^k$ for some $k in ZZ$. By [[Generators of Finite Cyclic Groups]] $b^k$ generates $\langle b \rangle$ if and only if $\gcd(|b|,k) = 1$, and $\varphi(d)$ counts for how many $0<k lt.eq |b|$ that holds (if $k>|b|$ by [[Equality of different exponents criterion]] $b^k$ is equal to some $b^j$ for $0<j lt.eq |b|$).