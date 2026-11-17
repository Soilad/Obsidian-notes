# Non-Inverting Amp $\left(V_{o} = \left(1+\frac{R_{F}}{R_{1}}\right)V_{in}\right)$
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) node[op amp, noinv input up](OA){}
  (OA.+) to[short, -o] ++(-1.5,0) node[left]{$V_{in}$}
  (OA.-) -- ++(0,-1.5) coordinate(FB)
  (FB) to[R=$R_1$, *-] ++(0,-2) node[ground]{}
  (FB) to[R=$R_F$] (FB -| OA.out) to[short, -*] (OA.out)
  (OA.out) to[short, -o] ++(1,0) node[right]{$V_o$};
\end{circuitikz}
\end{document}
```

# Inverting Amp $\left(V_{o} = -\frac{R_{F}}{R_{1}}V_{in}\right)$
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) node[op amp, noinv input down](OA){}
  (OA.-) -- ++(-0.5,0) coordinate(J)
  (J) to[R=$R_1$, *-o] ++(-2.5,0) node[left]{$V_{in}$}
  (J) -- ++(0,1.5) coordinate(FB)
  (FB) to[R=$R_F$] (FB -| OA.out) to[short, -*] (OA.out)
  (OA.out) to[short, -o] ++(1,0) node[right]{$V_o$}
  (OA.+) -- ++(0, -1) node[ground]{};
\end{circuitikz}
\end{document}
```

# Buffer / Voltage Follower $\left(V_{o} = V_{in}\right)$
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) node[op amp, noinv input up](OA){}
  (OA.+) to[short, -o] ++(-1.5,0) node[left]{$V_{in}$}
  (OA.-) -- ++(0,-1.2) coordinate(FB)
  (FB) -- (FB -| OA.out) to[short, -*] (OA.out)
  (OA.out) to[short, -o] ++(1,0) node[right]{$V_o$};
\end{circuitikz}
\end{document}
```

# Adder Amp $\left( V_{o} = -R_{F}\sum_{i}{\frac{V_{i}}{R_{i}}} \right)$
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) node[op amp, noinv input down](OA){}
  (OA.-) -- ++(-0.5,0) coordinate(J)
  % three inputs all meeting at the virtual-ground node J
  (J) to[R=$R_2$, *-o] ++(-3,0) node[left]{$V_2$}
  (J) -- ++(0,1.5) coordinate(A)
  (A) to[R=$R_1$, *-o] ++(-3,0) node[left]{$V_1$}
  (J) -- ++(0,-1.5) to[R=$R_3$, -o] ++(-3,0) node[left]{$V_3$}
  % feedback
  (A) -- ++(0,1.5) coordinate(FB)
  (FB) to[R=$R_F$] (FB -| OA.out) to[short, -*] (OA.out)
  (OA.out) to[short, -o] ++(1,0) node[right]{$V_o$}
  (OA.+) node[ground]{};
\end{circuitikz}
\end{document}
```

# Subtractor Amp $(V_{o} = V_{2}-V_{1})$
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) node[op amp, noinv input down](OA){}
  % inverting side
  (OA.-) -- ++(-0.5,0) coordinate(J)
  (J) to[R=$R$, *-o] ++(-3,0) node[left]{$V_1$}
  (J) -- ++(0,1.5) coordinate(FB)
  (FB) to[R=$R$] (FB -| OA.out) to[short, -*] (OA.out)
  (OA.out) to[short, -o] ++(1,0) node[right]{$V_o$}
  % non-inverting side (divider R2 / R3)
  (OA.+) -- ++(-0.5,0) coordinate(K)
  (K) to[R=$R$, *-o] ++(-3,0) node[left]{$V_2$}
  (K) to[R=$R$] ++(0,-2) node[ground]{};
\end{circuitikz}
\end{document}
```
