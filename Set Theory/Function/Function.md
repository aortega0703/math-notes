---
tags:
  - definition
  - math/set_theory
related topics:
  - "[[Set]]"
aliases:
  - Mapping
  - Domain
  - Image
  - Function composition
  - Graph
reference:
  - Gallian, J. A. Contemporary Abstract Algebra
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For [[Set|sets]] $A,B$
- A _function_ $f$ from $A$ to $B$ (denoted $f:A\to B$) assigns to each $a in A$ exactly one $b in B$ (in notation $f(a)=b$). It can be defined as a set $\Gamma_f \subseteq A\times B$ (its _graph_) such that $\forall a in A. \exists! b in B. (a,b) in \Gamma_f$ where $(a,b) in\Gamma_f  <==> f(a)=b$.
- The action of $f$ on some element $a$ is sometimes indicated as $a\mapsto f(a)$.
For a function $f:A\to B$ and some $a in A$
- $A$ is called the _domain_ of $f$.
- $B$ is called the _codomain_ of $f$.
- $f(a)$ is called the _image_ of $a$ under $f$.
---
- Function composition:
	For functions $A\overset{f}{\to}B\overset{g}{\to}C$ there is a function$$
	
		g\circ f: A &\to C\
		a &\mapsto g(f(a))
	
	$$
- Image of a subset of the domain:
	For a function $f:A\to B$ and $S\subseteq A$, the image of $S$ is defined as$$
		f(S) =\{f(a) in B\ |\ a in S\}\subseteq B
	$$
- Image of the function:
	For a function $f:A\to B$, the image of $f$ is defined as$$
		\operatorname{Im}(f) = \{f(a) in B: a in A\}\subseteq B
	$$Note that $f(A)=\operatorname{Im}(f)$.
- Preimage of a subset of the codomain:
	For a function $f:A\to B$ and $S\subseteq B$, the preimage of $S$ is defined as$$
		f^{-1}(S) = \{a in A: \exists b in B. f(a)=b\}\subseteq A
	$$Note that $f^{-1}(B)=A$. If $S=\{b\}$ then $f^{-1}(S)$ or simply $f^{-1}(b)$ is called the _fiber_ over $b$.
- Restriction of a function:
	For a function $f:A\to B$ and $A'\subseteq A$, the _restriction_ of $f$ to $A'$ ($f|_{A'}: S \to B$) is defined as$$
		f|_{A'}\ (a) = f(a)
	$$Note that $f|_{A'}=f\circ i$ where $i: A'\to A$ is an inclusion function.