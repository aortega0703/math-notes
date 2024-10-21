---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Dihedral group|Dihedral group]]"
---
$D_{2n}$ is precisely the group of symmetries of a regular $n$-gon, with $\sigma$ a clockwise rotation by $360\degree/n$ about the center, and $\tau$ a reflection about the line that passes through vertex $0$ and the center.
##### Proof:
Label the vertices of a regular $n$-gon clockwise from $0$ through $n-1$, such that vertex $k$ is next to vertex $k+1\ (\operatorname{mod}\ n)$.
- $D_{2n}\subseteq$ symmetries of a regular $n$-gon:
	Let $\sigma$ be a rotation by $360\degree/n$ about the center, and $\tau$ be a reflection about the line that passes through vertex $0$ and the center.
	- $\sigma$ is a symmetry:
		On a regular $n$-gon there is a vertex every $360\degree/n$ about the center, so $\sigma$ sends vertex $i$ (at $i\ 360\degree/n$) to position $i+1\ \operatorname{mod}\ n$ (at $(i+1)360\degree/n$) making it a symmetry. 
	- $\tau$ is a symmetry:
		On a regular $n$-gon there is a vertex every $360\degree/n$ about the center, so $\tau$ sends vertex $i$ (at $i\ 360\degree/n$) to position $-i\ \operatorname{mod}\ n$ (at $-i\ 360\degree/n$) making it a symmetry.
	- $\sigma^n=1$:
		$\sigma^n$ sends vertex $i$ (at $i\ 360\degree/n$) to
		$(i+n)(360\degree/n)=i\ 360\degree/n + 360\degree=i\ 360\degree/n$ so $\sigma^n$ is the identity symmetry.
	- $\tau^2=1$:
		$\tau^2$ sends vertex $i$ (at $i\ 360\degree/n$) to
		$-(-i)(360\degree/n)=i\ 360\degree$ so $\tau^2$ is the identity symmetry.
	- $\tau\sigma\tau=\sigma^{-1}$:
		$\tau\sigma\tau\sigma$ sends vertex $i$ (at $i\ 360\degree/n$) to $-(-(i+1)+1)\ 360\degree/n= i(360\degree/n)$, so $\tau\sigma\tau\sigma=1$ and $\tau\sigma\tau=\sigma^{-1}$.
	Then the elements of $D_{2n}$ are symmetries of a regular $n$-gon.
- $|$symmetries of a regular $n$-gon$|=|D_{2n}|$:
	- $|$symmetries of a regular $n$-gon$| = 2n$:
		Since symmetries are rigid, one that maps vertex $0$ to position $i$ also maps vertex $1$ to $i-1\ (\operatorname{mod}\ n)$ or $i+1\ (\operatorname{mod}\ n)$, so there are a total of $2n$ symmetries.
	- $|D_{2n}|=2n$:
		By [[Dihedral group order]].
Therefore $D_{2n}$ is the group of symmetries of a regular $n$-gon.