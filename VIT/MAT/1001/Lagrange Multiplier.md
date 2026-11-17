---
topic:
date: '"2026-11-16"'
course:
tags:
  - formula
---
> [[Gradient]] 
# Formula: $\nabla F=\lambda \nabla g$
$$
\begin{align}
\implies \frac{\partial F}{\partial x} &= \lambda \frac{\partial g}{\partial x}\\
\implies \frac{\partial F}{\partial y} &= \lambda \frac{\partial g}{\partial y}\\
\implies \dots
\end{align}
$$
# Tips:
> [!danger] 
usually you'll find cases like this
$2y = \lambda 2 y$
NEVER write it as
$1 = \lambda \frac{2y}{2y}$
Or involve variable division, as this doesn't account for when any of the variables could be 0
Instead, move everything towards one side and pull out common factors
$2y-\lambda 2 y = 0$
$\implies 2y (1-\lambda)= 0$
# Uses
- Finds Maxima and Minima
# Example
- 