---
tags:
  - theorem
  - complex_analysis
related topics:
  - Polar Form|Complex phase
  - "[[Polar Form]]"
---
For complex numbers $x=r_x(\cos\theta_x+i\sin\theta_x)$ and $y=r_y(\cos\theta_y+i\sin\theta_y)$, the norm of $xy$ is $r_x r_y$ and its phase is $\theta_x + \theta_y$.
##### Proof:
By [[Polar form exists]] $x=r_x(\cos\theta_x+i\sin\theta_x)$ and $y=r_y(\cos\theta_y+i\sin\theta_y)$. By [[Product of cosines]] $$
\cos\theta_x\cos\theta_y 
= \frac{1}{2}\big(\cos(\theta_x-\theta_y) 
+ \cos(\theta_x+\theta_y)\big)$$By [[Product of sines]]$$
\sin\theta_x\sin\theta_y 
= \frac{1}{2}\big(\cos(\theta_x-\theta_y)
- \cos(\theta_x+\theta_y)\big)$$By [[Cosine sine product]]$$
\begin{align}
	\cos\theta_x\sin\theta_y 
		&= \frac{1}{2}\big(\sin(\theta_x+\theta_y)
		- \sin(\theta_x- \theta_y)\big)\\
	\sin\theta_x\cos\theta_y
		&= \frac{1}{2}\big(\sin(\theta_x+\theta_y)
		+ \sin(\theta_x- \theta_y)\big)\\
\end{align}
$$Then$$
\begin{align}
	\cos\theta_x\cos\theta_y 
		- \sin\theta_x\sin\theta_y 
		&= \cos(\theta_x+\theta_y)\\
	\cos\theta_x\sin\theta_y 
		+ \sin\theta_x\cos\theta_y
		&= \sin(\theta_x+\theta_y)
\end{align}$$Therefore$$
\begin{align}
	xy &= r_x r_y 
		(\cos\theta_x+i\sin\theta_x) 
		(\cos\theta_y+i\sin\theta_y)\\
	&= r_x r_y 
		\big(\!\cos(\theta_x+\theta_y)
		+i\sin(\theta_x+\theta_y)\big)
\end{align}
$$So the phase of $xy$ is $r_x r_y$ and its phase is $\theta_x + \theta_y$.