---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Division|Modulo]]"
  - "[[Factorial]]"
mathLink: $(n-1)!\equiv 1\ (\operatorname{mod}\ n)\implies n$ prime
---
For $(n>1)  in  ZZ$, if $(n − 1)! \equiv 1 \ (\operatorname{mod} n)$, then $n$ is prime.
##### Proof:
Let $n=pq$ for some $0 lt.eq p,q  lt.eq n$. By [[Product of Modulus]] $(n-1)!\equiv 1\ (\operatorname{mod}\ p)$, then as $(n-1)! \equiv 0\ (\operatorname{mod}\ p)$ for any $p<n$, it must be the case that $p=n$ or $p=1$ (as $1\equiv 0\ \operatorname{mod}\ 1$). Therefore $n$ is prime.