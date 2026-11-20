---
topic:
date: '"2026-11-16"'
course:
tags:
  - formula
---
# Formula: $J(u,v) = \frac{\partial (x, y)}{\partial (u, v)} = \begin{vmatrix}\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v}\\ \frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}\end{vmatrix}$

## For single variable function: 
> $\int f(x)dx = \int f(g(u)) g'(u)du$
## So for double variable function: 
> $\iint f(x, y)dxdy = \iint f(g(u, v), h(u, v)) |J|dudv$
> [[]]
# Tips
- $\frac{\partial (x, y)}{\partial (u, v)}$ gives a matrix where numerator args are row-wise and denominator args are column-wise
# Uses
- in $\frac{\partial (x, y)}{\partial (u, v)}$ the determinant thingy is such that (x, y) is row wise and (u, v) is column wise
# Example
- 