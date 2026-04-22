#### (dielectric constant):
- $\displaystyle \epsilon_r  = k\epsilon_0$
$$
\displaystyle
\begin{align}
C = \frac QV\\
E = \frac \sigma {\epsilon_0}\\
V = \frac {Qd}{A\epsilon_0}\\
C = \frac {A\epsilon_0}{d}\\
C = \frac {A\epsilon_r}{d}\\
\end{align}
$$
#### In Series
$\displaystyle \frac 1{C_{eff}} = \sum \frac 1{C_i}$
#### In Parallel
$\displaystyle C_{eff} = \sum C_i$
#### [[Potential Energy]] stored
$\displaystyle U = \frac {CV^2}2$
#### [[CR Circuit]]
### In [[Alternating Current]]
$$
\displaystyle
\begin{align}
Q=CV\\
\implies Q = CV_0\sin(\omega t)\\
\implies I = CV_0\omega\cos(\omega t)\\
\implies I_0 = CV_0\omega\\
\implies V_0 = \frac{I_0}{C\omega}\\
\implies V_0 = X_cI_0\\
\end{align}
$$
```desmos-graph
left=0; right=10;
top=2; bottom=-2;
---
y=0.7*\sin(x)
y=1.2*\cos(x)
```
