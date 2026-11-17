---
epoch: 1794157283396
mode: agent
backendId: claude
sessionId: "44779646-b7d8-4be0-a26d-9262003f9609"
topic: "can you rewrite the circuitikz stuff for OpAmps and explain…"
tags:
  - copilot-conversation
usage: '{"usedTokens":38373,"contextWindow":1000000,"inputTokens":2,"outputTokens":8,"cacheReadTokens":34505,"cacheWriteTokens":3858,"updatedAt":1794157334699}'
---

**user**: can you rewrite the circuitikz stuff for [[OpAmps]] and explain how to properly write it
[Timestamp: 2026/11/08 22:31:23]

**ai**: I rewrote all five diagrams in [[OpAmps]]. I haven't rendered them, so open the note and check that each one draws properly.

## What was wrong

- **Inverting amp:** the input went straight into the `−` pin with no $R_1$, and the `+` pin went through a resistor to ground. The formula was also upside down. It's $-\frac{R_F}{R_1}V_{in}$, not $-\frac{R_1}{R_F}$.
- **Buffer:** the `−` input was tied to ground as well as to the output. It should connect only to the output.
- **Adder:** the formula was flipped. It's $-R_F\sum \frac{V_i}{R_i}$. The `+` pin also had a stray $R_1$ to ground. Some lines like `(-2,1) to[short,o-] (-2,1)` drew from a point to the same point, so they drew nothing.
- **Subtractor:** the drawing was mostly the inverting amp copied over. $V_2$ was wired straight into a pin, and the heading had the wrong formula. It now has the proper $R_2$/$R_3$ divider on the `+` input.

## How to write circuitikz properly

**1. Place the op-amp first and give it a name**
```latex
(0,0) node[op amp, noinv input down](OA){}
```
`OA` is just a name you choose. Once it's placed you can refer to its pins: `OA.-`, `OA.+` and `OA.out`. The option `noinv input up` puts `+` on top, and `noinv input down` puts `−` on top. Choose whichever puts the feedback input on the side where the feedback loop goes. Feedback goes above the op-amp in the inverting circuits and below it in the non-inverting ones.

**2. Draw outward from the pins with relative moves**
`++(dx,dy)` means "move this far from where I am now." Using it means you don't have to work out absolute coordinates.
```latex
(OA.-) -- ++(-0.5,0) coordinate(J)
```
`coordinate(J)` saves that point under a name so you can come back to it later. This is how you draw branches: start a new path at `(J)` and draw from there.

**3. Components go in `to[...]`**
- `to[R=$R_1$]` draws a labelled resistor.
- `--` draws a plain wire.
- `to[short]` also draws a wire, but it can take end markers.

**4. End markers go at the end of the options**
The two characters around the hyphen set the start and end of the line:
- `*-` puts a solder dot at the start.
- `-o` puts an open terminal at the end.
- `*-o` does both.

Put dots only at real junctions where three or more wires meet.

**5. Use `-|` to line things up**
`(FB -| OA.out)` means the point at FB's height and OA.out's x position. That's why the feedback resistor ends exactly above or below the output pin.

**6. Things that don't connect**
- `node[ground]{}` draws the ground symbol.
- `node[left]{$V_1$}` adds a label.

**7. Obsidian TikZJax specifics**
- Every block needs `\usepackage{circuitikz}`, `\begin{document}` and `\end{document}`.
- End each `\draw` with a `;`.
- Write labels as `$V_1$`, with the dollar signs, inside the options.
- `%` comments work. Use them to mark sections of a bigger circuit, as in the adder and subtractor.

A good habit: build one branch at a time and check the render after each one. Positions are relative, so a single mistake shifts everything drawn after it.
[Timestamp: 2026/11/08 22:31:23]