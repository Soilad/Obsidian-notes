---
topic:
date: 2026-11-16
course: MAT1001
tags:
  - formula
---
> [[Curl]] [[Divergence]]
# Meaning:
- The gradient takes a scalar function $f(x,y,z)$ and returns a vector field $\vec\nabla f$ made of its partial derivatives.
- If a vector field $\vec F$ is conservative, there is a scalar function $\phi$ with $\vec F = \vec\nabla \phi$. This $\phi$ is the potential.
- Geometrically, $\vec\nabla f$ describes how steeply $f$ changes in each direction, like the slope of a surface.
- **Synonyms:**
	- Potential function
	- Scalar potential
# Formula: $\vec{\nabla} = \frac{\partial }{\partial x}\hat i + \frac{\partial}{\partial y}\hat j +\frac{\partial}{\partial z}\hat{k}$
- $\vec{\nabla} f = \frac{\partial f}{\partial x}\hat i + \frac{\partial f}{\partial y}\hat j +\frac{\partial f}{\partial z}\hat{k}$
# Tips
- the constant function from integration has the other constant function when u integrate it
- $\vec\nabla f$ points in the direction of steepest increase of $f$. Its length is the rate of that increase.
- $-\vec\nabla f$ points in the direction of steepest decrease of $f$.
- At a local maximum or minimum, $\vec\nabla f = \vec 0$.
- For a unit vector $\hat n$, $\vec\nabla f \cdot \hat n$ is the rate of change of $f$ in the direction of $\hat n$ (the directional derivative).
# Uses
- Finding the direction of steepest increase or decrease of a function at a point.
- Recovering a potential $\phi$ from a conservative field $\vec F = \vec\nabla\phi$.
# Example
## Recovering a Potential from Its Gradient
Given $f_x$, $f_y$, $f_z$, find $f$. Integrate one partial derivative at a time. Each integration leaves an unknown function, which the next partial derivative pins down.

$$
\begin{align}
f_{x} &= e^x\cos{y} + yz\\
f_{y} &= xz - e^x\sin{y}\\
f_{z} &= xy+z
\end{align}
$$

**Step 1: integrate $f_x$ with respect to $x$.** Treat $y$ and $z$ as constants. The constant of integration becomes a function $g(y,z)$:

$$
f(x,y,z) = \int f_x\,dx = e^x\cos{y} + xyz + g(y,z)
$$

**Step 2: use $f_y$ to find $g$.** Differentiate with respect to $y$ and set it equal to $f_y$:

$$
\frac{\partial f}{\partial y} = -e^x\sin{y} + xz + \frac{\partial g}{\partial y} = xz - e^x\sin{y}
$$

So $\frac{\partial g}{\partial y} = 0$, which means $g(y,z) = h(z)$ for some function $h$.

Now $f(x,y,z) = e^x\cos{y} + xyz + h(z)$.

**Step 3: use $f_z$ to find $h$.** Differentiate with respect to $z$:

$$
\frac{\partial f}{\partial z} = xy + h'(z) = xy + z
$$

So $h'(z) = z$, and integrating gives $h(z) = \frac{z^2}{2}$ (plus a constant, which can be dropped).

**Result:**

$$
f(x,y,z) = e^x\cos{y} + xyz + \frac{z^2}{2}
$$

**Check:** Taking the partials of this $f$ gives back $f_x$, $f_y$, and $f_z$, so the answer is correct.
