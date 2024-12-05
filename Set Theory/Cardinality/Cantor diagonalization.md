---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Cardinality]]"
  - "[[Real numbers]]"
  - "[[Natural numbers]]"
---
$|\mathbb{R}|>|\mathbb{N}|$ i.e. The [[Cardinality]] of the set of [[Real numbers]] $\mathbb{R}$ is strictly greater than the cardinality of the set of [[Natural numbers]].
##### Proof:
Suppose there is a [[Injectivity and surjectivity|Surjective]] function $\phi: \mathbb{N}\to [0,1]\subset\mathbb{R}$. Consider the real number (in binary form) $d=0.d_1d_2\dots$ such that$$
d_k =
\begin{cases}
	1 &\text{if $\phi(k)_k=0$}\\
	0 &\text{if $\phi(k)_k=1$}\\
\end{cases}
$$it follows that $d\neq \phi(k)$ for all $k\in\mathbb{N}$ as they differ in the $k^\text{th}$ position. This is a contradiction, so there is no way to enumerate all real numbers.