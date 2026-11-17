- Current going in a node = Current going out of a node

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) to[battery1, l=$V_1$] (0,3)
  to[R=$R_1$, i<^=$i_1$] (4,3) node[above=4pt]{$V_A$}
  to[R=$R_3$, i^>=$i_3$] (8,3)
  to[battery1, l_=$V_2$] (8,0) -- (0,0)
  (4,3) to[R=$R_2$, *-*, i>^=$i_2$] (4,0);
\end{circuitikz}
\end{document}
```
> For any node $\sum{I_i} = 0$
$$
\begin{align}
i_1 &= \frac{V_1-V_A}{R_1}\\
i_2 &= \frac{V_A}{R_2}\\
i_3 &= \frac{V_2+V_A}{R_3}\\
0 &= i_1 + i_2 + i_3
\end{align}
$$
