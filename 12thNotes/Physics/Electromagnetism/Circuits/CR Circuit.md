[[Ohms Law]]
![[CR_Circuit.circuit-sketcher]]
```graph
bounds: [0, 1.2, 10, -0.2]
elements:
  - type: functiongraph
    def: ["f:1-exp(-x)"]
    att: {name: "1 − e^(−x)", withLabel: true, strokeColor: "blue"}
  - type: functiongraph
    def: ["f:exp(-x)"]
    att: {name: "e^(−x)", withLabel: true, strokeColor: "red"}
```
## From [[Kirchhoff Voltage Law]]
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
## [[Reactance]]
$\displaystyle X_c = \frac1{C\omega}$