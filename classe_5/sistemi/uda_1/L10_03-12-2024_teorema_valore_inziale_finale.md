# Teorema del valore iniziale e finale  

Il teorema ci permette di trovare i valori iniziali e finali di una funzione conoscendone la trasformata. In generale e' dimostrabile che:  

$\displaystyle{\lim_{t\to 0}\ f(t) = \lim_{s\to+\infty}\ s\cdot F(s)}$  

$\displaystyle{\lim_{t\to +\infty}\ f(t) = \lim_{s\to 0}\ s\cdot F(s)}$  

E' possible applicare il teorema ogni volta che i poli di $F(s)$ sono di ordine uno. Ovvero i fattori al denominatore (previa scomposizione se necessaria) hanno grado uno e.g.  

$F(s) = \dfrac{1}{(s+3)^1\cdot(s+5)^1}$  

## Esempio  

Considerando il transitorio di riscaldamento di un forno.  

$T(t) = 80u(t)-60e^{-0.05t}u(t)$  

Si ha allora che...  

$\displaystyle{\lim_{t\to 0}\ T(t) = 80-60 = 20^\circ C}$  
$\displaystyle{\lim_{t\to +\infty}\ T(t) = 80-0 = 80^\circ C}$  

Mentre nel dominio di Laplace...  

$T(t) \implies T(s) = \dfrac{80}{s}-\dfrac{60}{s+0.05}$  

$T(s) = \dfrac{80(s+0.05)-60s}{s(s+0.05)}=\dfrac{80s+4-60s}{s(s+0.05)} = \dfrac{20s+4}{s(s+0.05)}$  

Dal teorema del valore iniziale si ha allora che:  

$\displaystyle{\lim_{s\to +\infty}\ s\cdot T(s) = \cancel{s}\cdot\dfrac{20s+4}{\cancel{s}(s+0.05)}=\dfrac{\cancel{s}(20+\frac{4}{s})}{\cancel{s}(1+\frac{0.05}{s})}=\dfrac{20}{1} = 20^\circ C}$  

Mentre dal teorema del valore finale...  

$\displaystyle{\lim_{s\to 0}\ s\cdot T(s)=\cancel{s}\cdot\dfrac{20s+4}{\cancel{s}(s+0.05)}}=\dfrac{4}{0.05}=80^\circ C$  
