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
#### LC Circuit
![[RC_Circuit.circuit-sketcher]]
```desmos-graph
left=0; right=10;
top=1; bottom=0;
---
y=1-e^{-x}
y=e^{-x}
```
$$
\begin {align}
V - \frac QC - IR = 0\\
\implies V - \frac QC - \frac{dQ}{dt}R = 0\\
\implies \frac VR - \frac Q{RC} - \frac{dQ}{dt} = 0\\
\implies \frac Q{RC} + \frac{dQ}{dt} = \frac VR\\
\implies \frac Q{RC} + \frac{dQ}{dt} = \frac VR\\
\implies \mu = e^{(\int \frac{dt}{RC})} = e^{\frac t {RC}}\\
\implies Qe^{\frac t{RC}} = \frac VR \int e^{\frac t{RC}} dt\\
\implies Qe^{\frac t{RC}} = V(C e^{\frac t{RC}} + C_1)\\
\implies Q(t) = V(C + C_1 e^{\frac {-t}{RC}})\\
\implies Q(0) = V(C + C_1)\\
\implies C_1 = -C\\
\implies Q(t) = VC(1 - e^{\frac {-t}{RC}})\\
\implies Q(t) = Q_f(1 - e^{\frac {-t}{RC}})\\
\implies I(t) = \frac{Q_f}{RC}e^{\frac {-t}{RC}}\\
\end {align}
$$
#### [[Reactance]]
$\displaystyle X_c = \frac1{C\omega}$
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
