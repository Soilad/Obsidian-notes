Take a function
```desmos-graph
y=x^2
```
Hello function :)
### Moving along x-axis
> NOTE: k is -ve here to make it more consistent with moving it along y axis
- In order to move a function $f(x)$ along the x-axis, a constant to $x$ must added before it gets passed into $f$
- $\implies f(x-k); k=constant$ moves the graph of $f(x)$ along x-axis
	- $k > 0 \implies f(x-k)$ goes in +x-axis
	- $k < 0 \implies f(x-k)$ goes in -x-axis
```desmos-graph
k_1=2
k_2=-3
y=(x-k_1)^{2}
y=(x-k_2)^{2}
```

### Moving along y-axis
- In order to move a function $f(x)$ along the y-axis, a constant must added after  $f(x)$
- $\implies f(x)+k; k=constant$ moves the graph of $f(x)$ along x-axis
	- $k > 0 \implies f(x+k)$ goes in +y-axis
	- $k < 0 \implies f(x+k)$ goes in -y-axis
```desmos-graph
k_1=2
k_2=-3
y=(x)^{2}+k_1
y=(x)^{2}+k_2
```
### In combination
- to move a function $f$ 's vertex to coordinates $(x_0,y_0) \implies f(x-x_0)+y_0=y$
- Very useful to find where a function's vertex is highkey
### Example
- $y=x^2+2x$ 
- by solving the square we can write it as
$$
\displaystyle
\begin{align}
y=x^2+2x+1-1\\
\implies y=(x^2+2x+1)-1\\
\implies y=(x+1)^2-1\\
\end{align}
$$
- Now we know that this function's minima is at (-1, -1) (Yaya)
```desmos-graph
y=x^2+2x
```