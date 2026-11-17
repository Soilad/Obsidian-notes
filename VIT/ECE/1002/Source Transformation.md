```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) to[V, l=$V$, invert] (0,3)
  to[R=$R$, -o] (3,3)
  (0,0) to[short, -o] (3,0);
\draw[->] (4,1.8) -- (6,1.8);
\draw[<-] (4,1.2) -- (6,1.2);
\draw
  (7,0) to[I, l=${I = V/R}$] (7,3)
  -- (11,3) node[ocirc]{}
  (9,3) to[R=$R$, *-*] (9,0)
  (7,0) to[short, -o] (11,0);
\end{circuitikz}
\end{document}
```
