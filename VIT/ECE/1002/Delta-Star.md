> could also use [[Kirchhoff Current Law]] for this
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\coordinate (A) at (0,6);
\coordinate (B) at (7,6);
\coordinate (C) at (3.5,0);
\coordinate (O) at (3.5,3.6);
\draw
  (A) to[R=$R_{AB}$, *-*] (B)
  (B) to[R=$R_{BC}$, -*] (C)
  (C) to[R=$R_{AC}$] (A)
  (A) to[R=$R_A$, -*] (O)
  (B) to[R, l_=$R_B$] (O)
  (O) to[R=$R_C$] (C);
\node[left] at (A) {$A$};
\node[right] at (B) {$B$};
\node[below] at (C) {$C$};
\end{circuitikz}
\end{document}
```
### For $R_A, R_B, R_C$
$$
\begin{align}
R_A = \frac{R_{AC}R_{AB}}{R_{AB}+R_{BC}+R_{CA}}\\
R_B = \frac{R_{BC}R_{AB}}{R_{AB}+R_{BC}+R_{CA}}\\
R_C = \frac{R_{AC}R_{BC}}{R_{AB}+R_{BC}+R_{CA}}\\
\end{align}
$$
### For $R_{AB}, R_{BC}, R_{CA}$
$$
\begin{align}
R_{AB} = \frac{R_AR_B+R_AR_C+R_BR_C}{R_C}\\
R_{BC} = \frac{R_AR_B+R_AR_C+R_BR_C}{R_A}\\
R_{AC} = \frac{R_AR_B+R_AR_C+R_BR_C}{R_B}\\
\end{align}
$$
