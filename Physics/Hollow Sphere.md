> instead of having smthng like $x$ be the height of the ring its the arclength of $\theta$
$$
\displaystyle
\begin{align}
A = 2\pi r Rd\theta \\
dm = \frac M{4\pi R^2} 2\pi R^2 \sin(\theta) d\theta \\
\implies dm = \frac M{2}\sin(\theta) d\theta \\
I = \frac M{2} R^2 \int_0^\pi \sin^2(\theta)\sin(\theta) d\theta \\
\implies I = \frac M{2} R^2 \int_0^\pi (1-\cos^2(\theta))\sin(\theta) d\theta \\
u = \cos(\theta); du = -\sin(\theta)d\theta
\implies I = \frac M{2} R^2 [(u-\frac{u^3}3]_0^\pi\\
\implies I = - \frac M{2} R^2 [\cos(\theta)-\frac{\cos^3(\theta)}3]_0^\pi\\
\implies I = - \frac M{2} R^2 [
(-1+\frac 13)-
(1-\frac 13)
]\\
\implies I = - \frac M{2} R^2 2[(\frac {-2}3)]\\
\implies I = M R^2 \frac {2}3\\
\end{align}
$$