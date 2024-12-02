---
tags:
  - theorem
  - abstract_algebra
  - category_theory
related topics:
  - "[[Category of abelian groups]]"
  - "[[Direct product]]"
  - "[[Coproduct]]"
---
For [[Abelian group|Abelian groups]] $A,B$, their [[Direct product]] $A\times B$ is a [[Coproduct]] in $\mathbf{Ab}$ with the functions$$
\begin{align}
	\begin{aligned}
		\iota_A : A &\to A\times B\\
		a &\mapsto (a, e_B)
	\end{aligned}\qquad
	\begin{aligned}
		\iota_B : B &\to A\times B\\
		b &\mapsto (e_A, b)
	\end{aligned}
\end{align}
$$
##### Proof:
![[coproduct.png]]

Consider homomorphisms $\phi: A \to X$ and $\psi: B\to X$ and the function$$
\begin{align}
	\phi\cdot\psi : A\times B &\to X\\
    (a,b) &\mapsto \phi(a)\psi(b)
\end{align}
$$

- $\iota_A$ and $\iota_B$ are homomorphisms:
  Let $a_1,a_2\in A$, then$$
  \begin{align}
    \iota_A(a_1 a_2)
    &= (a_1 a_2, e_B)\\
    &= (a_1, e_B)\cdot(a_2, e_B)\\
    &= \iota_A(a_1)\cdot \iota_A(a_2)
  \end{align}
  $$Which makes $\iota_A$ an homomorphism, similarly with $\iota_B$.
- $\phi\cdot\psi$ is an homomorphism:
  Let $a_1,a_2\in A$ and $b_1, b_2\in B$. Then$$
  \begin{align}
    (\phi\cdot\psi)\big((a_1,b_1)\cdot(a_2, b_2)\big)
    &= (\phi\cdot\psi)(a_1 a_2,b_1 b_2)\\
    &= \phi(a_1 a_2) \psi(b_1 b_2)\\
    &= \phi(a_1) \phi(a_2) \psi(b_1)\psi(b_2)\\
    &= \phi(a_1) \psi(b_1) \phi(a_2) \psi(b_2)\\
    &= (\phi\cdot\psi)(a_1,b_1) \cdot (\phi\cdot\psi)(a_2,b_2)
  \end{align}
  $$making $\psi\cdot\psi$ an homomorphism. Note that this is not necessarily true when $X$ is no abelian as we need $\phi(a_2)$ and $\psi(b_1)$ to commute.
- $A\times B$ is a coproduct:
  Let $a\in A$, then$$
  \begin{align}
    (a)\iota_A(\phi\cdot\psi)
    &= (a,e_B)(\phi\cdot\psi)\\
    &= \phi(a) \psi(e_B)\\
    &= \phi(a) e_X\\
    &= \phi(a)
  \end{align}
  $$So by extensionality $\iota_A(\phi\cdot\psi) = \phi$. Similarly $\iota_B(\phi\cdot\psi) = \psi$.
Then $A\times B$ is a coproduct in $\mathbf{Ab}$.