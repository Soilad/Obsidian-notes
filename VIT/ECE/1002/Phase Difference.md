```tikz
\usepackage{tikz}
\begin{document}
\begin{tikzpicture}[scale=1.2, >=latex]
% Axes
\draw[->, gray] (-0.5,0) -- (4.5,0) node[right] {Re};
\draw[->, gray] (0,-2) -- (0,2.5) node[above] {Im};

% Voltage phasor (reference)
\draw[->, very thick, blue] (0,0) -- (4,0) node[below right] {$\vec{V}$};

% Current phasor (lagging by phi)
\draw[->, very thick, red] (0,0) -- (-30:3) node[below right] {$\vec{I}$};

% Angle phi
\draw[->] (1.2,0) arc (0:-30:1.2);
\node at (-15:1.55) {$\phi$};
\end{tikzpicture}
\end{document}
```
- $= \tan^{-1}{(\frac{|{V_{C}}-V_{L}|}{V_{R}})}$
- $= \tan^{-1}{(\frac{|{X_{C}}-X_{L}|}{R})}$