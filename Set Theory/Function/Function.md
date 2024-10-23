---
tags:
  - definition
  - set_theory
related topics:
  - "[[Set]]"
aliases:
  - Mapping
  - Domain
  - Image
  - Function composition
reference:
  - Gallian, J. A. Contemporary Abstract Algebra
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For [[Set|sets]] $A,B$
- A _function_ $f$ from $A$ to $B$ (denoted $f:A\to B$) assigns to each $a\in A$ exactly one $b\in B$ (in notation $f(a)=b$). It can be defined as a set $\Gamma_f \subseteq A\times B$ such that $\forall a\in A. \exists! b\in B. (a,b)\in \Gamma_f$.
- The action of $f$ on some element $a$ is sometimes indicated as $a\mapsto f(a)$.
For a function $f:A\to B$ and some $a\in A$
- $A$ is called the _domain_ of $f$.
- $B$ is called the _codomain_ of $f$.
- $f(a)$ is called the _image_ of $a$ under $f$.
For functions $f:A\to B$ and $g:B\to C$
- The _composition_ $g\circ f: A\to C$ is defined as $(g\circ f)(a)=g(f(a))$.
---
- Evaluating on a subset of the domain:
	For a function $f:A\to B$ and $A'\subseteq A$, the image of $A'$ is defined as$$
		f(A') =\{f(a)\in B\ |\ a\in A'\}\subseteq B
	$$
- Image of the function:
	For a function $f:A\to B$, the image of $f$ is defined as$$
		\operatorname{Im}(f) = \{f(a)\in B: a\in A\}\subseteq B
	$$Note that $f(A)=\operatorname{Im}(f)$.
- Inclusion function:
	For sets $A\subseteq B$, there is an inclusion function $A\to B$ defined as $a\mapsto a$.
- Identity function:
	For a set $S$, its _identity_ or _diagonal_ function ($\operatorname{id}_S: S \to S$) is defined as$$\operatorname{id}_S(s) =s$$Note that $\operatorname{id}_S$ is an inclusion function with equal domain and codomain.
- Restriction of a function:
	For a function $f:A\to B$ and $A'\subseteq A$, the _restriction_ of $f$ to $A'$ ($f|_{A'}: S \to B$) is defined as$$
		f|_{A'}\ (a) = f(a)
	$$Note that $f|_{A'}=f\circ i$ where $i: A'\to A$ is an inclusion function.