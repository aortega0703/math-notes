---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Category of sets]]"
  - "[[Initial-final object|Initial object]]"
---
In the [[Category]] $\mathbf{Set}$, $\emptyset$ is its only [[Initial-final object|Initial object]].
##### Proof:
- $\emptyset$ is initial:
	By definition a function $f:\emptyset\to B$ can be viewed as its [[Function|Graph]] $\Gamma_f\subseteq \emptyset\times B=\emptyset$. The requirements for $\Gamma_f=\emptyset$ being a graph are fulfilled vacuously, that is$$
	\forall a\in\emptyset.\exists!b\in B.(a,b)\in\Gamma_f
	$$is true as there are no $a\in \emptyset$. As there is a single function $\emptyset\to B$ for all objects $B$ (corresponding to the empty graph) $\emptyset$ is initial in $\mathbf{Set}$.
- There are no other initial objects:
	Let $A\neq \emptyset$, by definition a function $f:A\to\emptyset$ can be viewed as its [[Function|Graph]] $\Gamma_f\subseteq A\times\emptyset=\emptyset$. The requirements for $\Gamma_f=\emptyset$ being a graph are not fulfilled however, that is$$
	\forall a\in A.\exists!b\in \emptyset.(a,b)\in\Gamma_f
	$$is false as there are no such $b\in\emptyset$. Therefore $\emptyset$ is the only initial object in $\mathbf{Set}$.