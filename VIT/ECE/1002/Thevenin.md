```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
% Nodes: A (top), B (left), C (right), D (bottom)
\coordinate (A) at (3,6);
\coordinate (B) at (0,3);
\coordinate (C) at (6,3);
\coordinate (D) at (3,0);

% Bridge arms
\draw (A) to[R, l_=$R_1$, *-*] (B);
\draw (A) to[R, l=$R_2$, -*] (C);
\draw (B) to[R, l_=$R_3$, -*] (D);
\draw (C) to[R, l=$R_4$] (D);

% Galvanometer across B–C
\draw (B) to[R, t=G, l=$R_l$] (C);

% Source from A to D
\draw (A) -- (3,7) -- (-2,7)
      to[battery1, l_=$V$] (-2,-1) -- (3,-1) -- (D);

% Node labels
\node[left] at (B) {$V_{A}$};
\node[right] at (C) {$V_{B}$};
\end{circuitikz}
\end{document}
```
# $R_{{th}}$:
- **Voltage Sources:** Short Circuit
- **Current Sources:** Open Circuit
```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
% Nodes: A (top), B (left), C (right), D (bottom)
\coordinate (A) at (3,6);
\coordinate (B) at (0,3);
\coordinate (C) at (6,3);
\coordinate (D) at (3,0);

% Bridge arms
\draw (A) to[R, l_=$R_1$, *-*] (B);
\draw (A) to[R, l=$R_2$, -*] (C);
\draw (B) to[R, l_=$R_3$, -*] (D);
\draw (C) to[R, l=$R_4$] (D);

% Galvanometer across B–C
% \draw (B) to[R, t=G, l=$R_l$] (C);

% Source from A to D
\draw (A) -- (D);

% Node labels
\node[left] at (B) {$V_{A}$};
\node[right] at (C) {$V_{B}$};
\end{circuitikz}
\end{document}

```
$R_{th} = (R_{1}\parallel R_{2})+(R_{3}\parallel R_{4})$
# $V_{th}$ :
- $V_{th}= V_{A} - V_{B}$
> If there's a reference node use [[KCL]] from one end to the reference node