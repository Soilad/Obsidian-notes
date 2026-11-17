```_graph
y = 4*max(sin(x), 0)
```
- $V_{avg} = \frac{V_{max}}{\pi}$
- $V_{rms} = \frac{V_{max}}{2}$
- $FF = \frac{\pi}{2}$
```_graph
y = 4*abs(sin(x))
```
- $V_{avg} = \frac{2V_{max}}{\pi}$
- $V_{rms} = \frac{V_{max}}{2\sqrt{2}}$
- $FF = \frac{\pi}{2\sqrt{2}}$
```_graph
y = 4*round(sin(x)^2)
```
- $V_{avg} = Magn.\frac{T_{on}}{T}$
- $V_{rms} = \sqrt{Magn.^2\frac{T_{on}}{T}}$
```_graph
y = 4*round(sin(x)^2)
```
- $V_{avg} = Magn.\frac{T_{on}}{T}$
- $V_{rms} = \sqrt{Magn.^2\frac{T_{on}}{T}}$
```_system
y = |sin(x)| * max(sign(x % pi - 1), 0)
y = |sin(x)|
```
- $V_{avg} = \frac{2V_{max}}{\pi}*(1+\cos{\alpha})$