# Teorema del valore iniziale e finale  

E' possibile dimostrare che, data una funzione nel dominio di Laplace $F(s)$, si puo' ricavare il valore iniziale $f_i$ e quello finale $f_f$ con:  

$$
f_i = \lim_{s \to +\infty} F(s)\cdot s
$$

$$
f_f = \lim_{s \to 0}\ F(s)\cdot s
$$

Data la funzione di trasferimento $G(s) = \dfrac{s}{s+4}$ e la funzione in ingresso $x(t) = 10 \cdot u(t)$ e' possibile allora ritrovare il valore finale e quello iniziale.  

$x(t) = 10 \cdot u(t) \implies X(s) = \dfrac{10}{s}$  

$Y(s) = G(s)X(s) = \dfrac{\cancel{s}}{s+4} \cdot \dfrac{10}{\cancel{s}}= \dfrac{10}{s+4}$  

Applichiamo allora il **teorema del valore iniziale** manipolando i termini in modo da togliere di mezzo la $s$ al numeratore, e notando infine che quando $s$ diventa molto grande $\frac{4}{s}$ diventa un numero $x$ molto piccolo che si avvicina a zero senza mai raggiungerlo, ma essendo comunque molto piccolo e' possible ignorarlo.  

$f_i = \underset{s \to +\infty}{\lim} Y(s)\cdot s = \dfrac{10}{s+4} \cdot s = \dfrac{10\cancel{s}}{\cancel{s}(1+\frac{4}{s})} = \dfrac{10}{1 + x} = \dfrac{10}{1} =10$  

Lo stesso vale per il **teorema del valore finale** dove la $s$ tende a zero scomparendo al denominatore e trasformando il numeratore in un numero $x$ che tende a zero.  

$f_f = \underset{s \to 0}{\lim}\ Y(s)\cdot s = \dfrac{10}{s+4} \cdot s = \dfrac{10 \cdot s}{4} = \dfrac{x}{4} = 0$  

Infine tornando al dominio del tempo si puo' notare come i risultati ottenuti dai teoremi siano in accordo.  

$Y(s) = \dfrac{10}{s+4} \implies y(t) = 10 \cdot e^{-4t}u(t)$  

![function_plot_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1d1d089e-af5f-4179-b057-c72e592c0be1)  
