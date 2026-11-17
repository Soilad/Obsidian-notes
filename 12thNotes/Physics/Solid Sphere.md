> NOTE: $dI$ is half of the expected $mr^2$ as $r$ changes
$$
\displaystyle
\begin{align}
x = R\sin(\theta)\\
r = R\cos(\theta)\\
r = R\cos(\arcsin(\frac xR))\\
r = R\sqrt{1^2-\frac {x^2}{R^2}}\\
r = \sqrt{R^2-x^2}\\
m = \rho \pi r^2 x \\
dm = \rho \pi r^2 dx \\
\implies dm = \rho \pi (R^2-x^2) dx \\
\implies dI = \frac {\rho \pi}2  (R^2-x^2)(R^2-x^2) dx \\
\int dI = \frac {\rho \pi}2 \int_{-R}^R (R^2-x^2) (R^2-x^2) dx\\
\implies I = \frac {\rho \pi}2 \int_{-R}^R R^4+x^4-2(xR)^2dx\\
\implies I = \frac {\rho \pi}2 [R^4x+\frac {x^5}5-2R^2\frac {x^3}3]_{-R}^R\\
\implies I = \frac {\rho \pi}2 [
(R^5+\frac {R^5}5-\frac 23R^5)
- (-R^5-\frac {R^5}5+\frac 23R^5)
]\\
\implies I = \rho \pi [R^5+\frac {R^5}5-\frac 23R^5]\\
\implies I = \rho \pi R^5[1+\frac 15-\frac 23]\\
\implies I = \rho \pi R^5[\frac {15+3-10}{15}]\\
\implies I = \rho \pi R^5[\frac {8}{15}]\\
\implies I = \frac{m}{\frac 43 \pi R^3} \pi R^5[\frac {16}{15}]\\
\implies I = \frac{3m}{4 \pi} \pi R^2[\frac {8}{15}]\\
\implies I = \frac {2}{5} mR^2\\
\end{align}
$$