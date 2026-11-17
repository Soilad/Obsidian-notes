```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) to[battery1, l=$V$] (0,3)
  -- (4.5,3)
  (2,3) to[R=$R_1$, *-*] (2,0)
  (4,3) to[R=$R_2$, *-*] (4,0)
  (4.5,0) -- (0,0);
\node at (5,1.5) {$\cdots$};
\end{circuitikz}
\end{document}
```
### In Parallel Circuit
- $V = V_1 = V_2$ ($V$ is constant) 
- $I = I_1 + I_2$ (from [[Kirchhoff Current Law]])
$$
\begin{align}
V_1 = I_1R_1\\
V_2 = I_2R_2\\

\implies I_1 = \frac{V_1}{R_1}\\
\implies I_2 = \frac{V_2}{R_2}\\
\implies I = \frac{V_1}{R_1} + \frac{V_2}{R_2}\\
\implies V(\frac{1}{R_1}+\frac{1}{R_2}) = V\frac{1}{R_{eq}}\\
\implies \frac{1}{R_{eq}} = \sum{\frac{1}{R_i}}\\
\implies C_{eq} = \sum{C_i}\\
\end{align}
$$
### For Any $I_n$
$$
\begin{align}
I = \frac{V_n}{R_n}\\
\implies I_n = I\frac{R_n}{R_{eq}}\\
\end{align}
$$
