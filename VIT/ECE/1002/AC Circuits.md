```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
% Source and series resistor
\draw (0,0) to[sV, l=$v_s(t)$] (0,4)
      to[R, l=$R_1$, i>^=$i_s$, -*] (4,4);

% Branch 1: inductor
\draw (4,4) to[L, l_=$L$, i>^=$i_L$, -*] (4,0);

% Branch 2: capacitor + resistor
\draw (4,4) -- (8,4)
      to[C, l=$C$, i>^=$i_C$] (8,2)
      to[R, l=$R_2$] (8,0) -- (4,0);

% Return path
\draw (4,0) -- (0,0);

% Output across the parallel section
\draw (4,4) -- (5,4);
\node[above] at (4,4) {$a$};
\node[below] at (4,0) {$b$};
\end{circuitikz}
\end{document}
```
# For Resistors: $R_{eq} = R_{i}$
# For Inductors: $R_{eq} = jX_{L}$
# For Conductors: $R_{eq} = -jX_{C}$
[[Reactance]]