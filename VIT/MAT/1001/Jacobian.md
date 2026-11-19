---
topic:
date: '"2026-11-16"'
course:
tags:
  - formula
---
<errorChunk>Model request failed: No chat model enabled. Enable a model under Settings → Basic → Agents → Quick Chat, or add one on the BYOK tab.</errorChunk># Formula: $J(u,v) = \begin{vmatrix}\frac{\partial x}{\partial u} & \frac{\partial x}{\partial v}\\ \frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}\end{vmatrix} = \frac{\partial (x, y)}{\partial (u, v)}$

## For single variable function: 
> $\int f(x)dx = \int f(g(u)) g'(u)du$
## So for double variable function: 
> $\iint f(x, y)dxdy = \iint f(g(u, v), h(u, v)) |J|dudv$
> [[]]
# Tips
-  
# Uses
- in $\frac{\partial (x, y)}{\partial (u, v)}$ the determinant thingy is such that (x, y) is row wise and (u, v) is column wise
# Example
- 