---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Order]]"
  - "[[Group]]"
  - "[[Euler's Phi Function|Euler's Totient Function]]"
---
In a finite group $G$, the number of elements of order $d$ is a multiple of $\varphi(d)$.
##### Proof:
- $G$ has no elements of order $d$:
	$0$ is a multiple of $\varphi(d)$.
- There is some $a\in G$ with $|a|=d$:
	- No element of order $d$ belongs to two different cyclic subgroups of order $d$:
		Suppose $b\in G - \langle a \rangle$ with $|b|=d$. If there is some $c\in \langle a \rangle \cap \langle b \rangle$ with $|c|=d$, then by [[Cyclic subgroup]] $\langle c\rangle \subseteq \langle a\rangle$ and $\langle c\rangle \subseteq \langle b\rangle$. By [[Order of cyclic group is order of generator]], $|\langle c \rangle|= |\langle a \rangle| = |\langle b \rangle| = d$ so $\langle c \rangle=\langle a \rangle = \langle b \rangle$ and $b\in \langle a \rangle$ which contradicts $b\in G-\langle a \rangle$, so there is no $\langle b \rangle$ of order $d$ that shares elements of order $d$ with $\langle a \rangle$.
	By [[Number of Elements of Each Order in Cyclic Group]] $\langle a \rangle$ has $\varphi(d)$ elements of order $d$. As no elements of $G$ with order $d$ belong to multiple cyclic subgroups of order $d$, the number of elements of order $d$ in $G$ is $k\varphi(d)$ with $k$ being the number of cyclic subgroups of order $d$.