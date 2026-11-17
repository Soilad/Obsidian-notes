---
topic:
date: '"2026-11-16"'
course:
tags:
  - formula
---
> [[Curl]] [[Divergence]]
# Meaning:
- Gives the slope vectors of a surface
- **Synonyms:**
	- Potential function
	- Scalar Potential
# Formula: $\vec{\nabla} = \frac{\partial }{\partial x}\hat i + \frac{\partial}{\partial y}\hat j +\frac{\partial}{\partial z}\hat{k}$
- $\vec{\nabla} f = \frac{\partial f}{\partial x}\hat i + \frac{\partial f}{\partial y}\hat j +\frac{\partial f}{\partial z}\hat{k}$
# Tips
- $\vec\nabla F$ gives a vector pointing towards local maxima
- $-\vec\nabla F$ gives a vector pointing towards local minima
- $\vec\nabla F \cdot \hat n$ gives a directional derivative along $\vec n$
# Uses
- Gives you a function returns a vector pointing to the local maxima
# Example
## Gradient to Surface
$$
\begin{align}

f(x,y,z) &= ?\\
f_{x} &= e^x\cos{y} + yz\\
f_{y} &= xz - e^x\sin{y}\\
f_{z} &= xy+z\\
\implies f(x, y, z) &= \int{f_{x}}dx = e^x\cos{y} + xyz + g(y,z)\\
\implies \frac{d}{dy}f(x,y,z) &= f_{y}\\
\implies xz-e^x\sin{y} &= e^x-\sin{y}+xz + \frac{d}{dy}g(y,z)\\
\implies \frac{d}{dy}g(y,z) &= 0\\
\implies g(y,z) = \int{0}dy &= 0+h(z)\\
\implies f(x,y,z) = \int{f_{x}}dx &= e^x\cos{y} + xyz + h(z)\\
\implies \frac{d}{dz}f(x,y,z) = f_{z} &= xy + \frac{d}{dz}h(z)\\
\implies xy + z &= xy + \frac{d}{dz}h(z)\\
\implies h(z) &= \int{z}dz\\
\implies f(x,y,z) = \int{f_{x}}dx &= e^x\cos{y} + xyz + z\\

\end{align}
$$
