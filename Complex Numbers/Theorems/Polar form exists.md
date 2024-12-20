---
tags:
  - theorem
  - complex_analysis
  - needs_details
related topics:
  - "[[Complex numbers]]"
mathLink: $a+bi = r(\cos\theta + i\sin\theta)$
---
For any $x=a+bi\in\mathbb{C}$, it can be written as $x=r (\cos\theta + i \sin\theta)$ for some $r,\theta\in\mathbb{R}$.
##### Proof:
![[Complex polar form.png]]
As $1$ and $i$ are perpendicular it is possible to form a right triangle of sides $a$ and $b$ with hypotenuse $$r=\sqrt{a^2 + b^2}$$By [[Sin opposite hypotenuse]] and [[Cos adjacent hypotenuse]] $\sin\theta = b/r$ and $\cos\theta=a/r$, so$$
\begin{align}\theta = 
\begin{cases}
	\phantom{-}\operatorname{undefined} &\text{if $r=0$}\\
	\phantom{-}\arccos(a/r) &\text{if $b\geq0$}\\
	-\arccos(a/r) &\text{if $b<0$}\\
\end{cases}\\
\\
a=r\cos\theta\quad
b=r\sin\theta
\end{align}$$To check for equality see that$$
\begin{align}
	a + bi &= \frac{r}{r}(a+bi)\\
	&= r \left(\frac{a}{r} + i \frac{b}{r}\right)\\
	&= r \left(\cos\theta + i \sin\theta\right)\\
\end{align}
$$
