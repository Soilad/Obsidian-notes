$$
\begin{align}
V = V_0\sin(\omega t)\\
I = I_0\sin(\omega t)\\
\end{align}
$$
#### Root Mean Squared:
```graph
bounds: [0, 1.2, 10, -1.2]
elements:
  - type: functiongraph
    def: ["f:sin(x)"]
    att: {name: "alternating current", withLabel: true, strokeColor: "blue"}
  - type: functiongraph
    def: ["f:pow(sin(x), 2)"]
    att: {name: "sin²x", withLabel: true, strokeColor: "red"}
  - type: functiongraph
    def: ["f:0.5"]
    att: {name: "0.5", withLabel: true, strokeColor: "green", dash: 2}
  - type: functiongraph
    def: ["f:sqrt(0.5)"]
    att: {name: "√0.5 (rms)", withLabel: true, strokeColor: "purple", dash: 2}
```
- basically jst approximations the alternating value
[[CR Circuit]]
[[LCR Circuit]]