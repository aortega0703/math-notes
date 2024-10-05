---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Greatest Common Divisor|Relative Prime]]"
mathLink: $a=a'\gcd(a,b),\ b=b'\gcd(a,b) \implies \gcd(a',b')=1$
---
For $a,b\in \mathbb{Z}$, $a\ /\gcd(a,b)$ and $b\ /\gcd(a,b)$ are relative primes.
##### Proof:
Let $a=a' \gcd(a,b)$ and $b=b'\gcd(a,b)$ for some $a',b'\in\mathbb{Z}$. Also let $a'= a''\gcd(a',b')$ and $b'=b''\gcd(a',b')$ for some $a'',b''\in\mathbb{Z}$. Then $a=a''\gcd(a',b')\gcd(a,b)$ and $b=b''\gcd(a',b')\gcd(a,b)$ so $\gcd(a',b')\gcd(a,b)$ is a common divisor of $a$ and $b$, but $\gcd(a,b)$ is the greatest common divisor so $\gcd(a',b')=1$.