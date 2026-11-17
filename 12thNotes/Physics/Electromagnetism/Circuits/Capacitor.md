#### Dielectric constant:
- $\displaystyle \epsilon_r  = k\epsilon_0$
$$
\begin{align}
C &= \frac QV\\
E &= \frac \sigma {\epsilon_0}\\
V &= \frac {Qd}{A\epsilon_0}\\
C &= \frac {A\epsilon_0}{d}\\
C &= \frac {A\epsilon_r}{d}\\
\end{align}
$$
#### In [[Series]]
$\displaystyle \frac 1{C_{eff}} = \sum \frac 1{C_i}$
#### In [[Parallel]]
$\displaystyle C_{eff} = \sum C_i$
#### [[Potential Energy]] stored
$\displaystyle U = \frac {CV^2}2$
#### [[CR Circuit]]
#### [[LCR Circuit]]
### In [[Alternating Current]]
$$
\begin{align}
Q &= CV\\
\implies Q &= CV_0\sin(\omega t)\\
\implies I &= CV_0\omega\cos(\omega t)\\
\implies I_0 &= CV_0\omega\\
\implies V_0 &= \frac{I_0}{C\omega}\\
\implies V_0 &= X_cI_0\\
\end{align}
$$
```graph
bounds: [0, 2, 10, -2]
elements:
  - type: functiongraph
    def: ["f:0.7*sin(x)"]
    att: {name: "0.7 sin x", withLabel: true, strokeColor: "blue"}
  - type: functiongraph
    def: ["f:1.2*cos(x)"]
    att: {name: "1.2 cos x", withLabel: true, strokeColor: "red"}
```
