- Sum of Voltage in a loop = 0

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) to[battery1, l=$V_1$] (0,3)
  to[R=$R_1$] (4,3) coordinate(A)
  to[R=$R_3$] (8,3)
  to[battery1, l_=$V_2$] (8,0) -- (0,0)
  (A) to[R=$R_2$, *-*] (4,0);
\draw[->] (1.4,2) arc[start angle=150, end angle=-150, radius=0.6] node[midway, right]{};
\node at (2,1.5) {$I_1$};
\draw[->] (6.6,2) arc[start angle=30, end angle=330, radius=0.6];
\node at (6,1.5) {$I_2$};
\end{circuitikz}
\end{document}
```
> In a closed loop $\sum{V_i} = 0$
$$
\begin{align}
0 &= V_1 - IR_1 - IR_2\\
0 &= V_2 - IR_3 - IR_2\\
0 &= V_1 - IR_1 - IR_3 + V_2\\
\end{align}
$$
