#### [[Magnetic Flux]]
> L = Inductance
#### Self Induction:
- the EMF induced in itself due to change in current
- $\displaystyle \epsilon = -L \frac{dI}{dt}$
#### Mutual Induction:
- the EMF induced from one coil to another due to change in current
- $\displaystyle \epsilon = -M \frac{dI}{dt}$
#### Eddy Currents:
- its loops of current induced in conductors by changing magnetic field leading to energy loss as head
### In [[Alternating Current]]
$$
\begin{align}
\varepsilon &= -L\frac{dI}{dt}\\
\implies \varepsilon &= -L\frac{dI_0\sin(\omega t)}{dt}\\
\implies \varepsilon &= -LI_0\omega \cos(\omega t)\\
\end{align}
$$
```graph
bounds: [0, 2, 10, -2]
elements:
  - type: functiongraph
    def: ["f:0.7*cos(x)"]
    att: {name: "0.7 cos x", withLabel: true, strokeColor: "blue"}
  - type: functiongraph
    def: ["f:1.2*sin(x)"]
    att: {name: "1.2 sin x", withLabel: true, strokeColor: "red"}
```
#### [[Magnetic Dipole]]
#### [[Transformers]]
#### [[LCR Circuit]]