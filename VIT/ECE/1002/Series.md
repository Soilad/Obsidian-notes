```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[scale=0.8, transform shape]
\draw
  (0,0) to[battery1, l=$V$] (0,4)
  -- (3,4)
  to[R=$R_1$] (3,2)
  to[R=$R_2$] (3,0) -- (0,0);
\end{circuitikz}
\end{document}
```
### In Series Circuit
- $V = V_1 + V_2$ (from [[Kirchhoff Voltage Law]])
- $I = I_1 = I_2$ ($I$ is constant)
$$
\begin{align}
V_1 &= I_1R_1\\
V_2 &= I_2R_2\\
\implies V_1 &= IR_1\\
\implies V_2 &= IR_2\\
\implies V &= V_1 + V_2 = IR_1 + IR_2 \\
\implies V &= I(R_1 + R_2)\\
\implies R_{eq} &= (R_1 + R_2)\\
\implies R_{eq} &= \sum{R_i};\ \forall R_i\ in\ series\\
\end{align}
$$
### For Any $V_n$
$$
\begin{align}
V_n &= IR_n\\
\implies V_n &= \frac{V}{R_{eq}}R_n = V\frac{R_n}{R_{eq}}\\
\end{align}
$$
