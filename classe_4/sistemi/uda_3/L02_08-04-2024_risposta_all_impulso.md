# Risposta del sistema  

![rl_serie](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b7d4a96a-d2a4-41ac-81db-fc4cb2e75c8a)  

Si vuole trovare la tensione in uscita $V_L$ di questo circuito RL, dove $R = 10\ \Omega$ e $L = 2\ H$ mentre il segnale in ingresso e' un gradino unitario $v_{in}(t) = 1\ V \cdot u(t)$. Si nota allora come la risposta del sistema, ovvero la tensione in uscita $V_L(s)$ dipenda non solo dalla composizione del sistema stesso $G(s)$ ma anche dal segnale in ingresso $V_{in}(s)$.  

$V_{L}(s) = G(s) \cdot V_{in}$  

Dove per il partitore di tensione si ha che $G(s) = \dfrac{Ls}{R+Ls}$ si ha allora che:  

$V_L(s) = \dfrac{Ls}{R+Ls} \cdot V_{in}(s) = \dfrac{2\cancel{s}}{10+2s} \cdot \dfrac{1}{\cancel{s}} = \dfrac{\cancel{2}}{\cancel{2}(5+s)} = \dfrac{1}{5+s}$  

$V_L(s) \implies v_L(t) = e^{-5t} \cdot u(t)$  

![vl_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ccdd5b0b-d8e7-447d-bbbd-24414ac535a7)  

# Impulso unitario  

In questo constesto un **impulso generico** e' definito come un segnale rettangolare che mantiene un area unitaria $A = h \cdot \dfrac{1}{h}$  

$$
\delta_h(t) = \begin{cases}
  \begin{aligned}
    \dfrac{1}{h}&\ \ \ 0 \le t \le h  \\
    0&\ \ \ \ otherwise \\
  \end{aligned}
\end{cases}
$$

![generic_impulse](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1ca54712-9cf1-463d-baea-9ba2d18a8767)  

Si definisce invece **impulso unitario** (o *delta di Dirac*) una tensione enorme di brevissima durata, in particolare il limite dell'impulso generico con $h$ che tende a zero.  

$\delta(t) = \underset{h \to 0}{\lim}\ \delta_h(t)$  

![delta_dirac](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a61e9d6c-612a-4d71-900c-1fad20be14fa)  

Se $h \to 0$ allora $\dfrac{1}{h}$ diventa infinitamente grande, la freccia rappresenta prioprio il fatto che il valore tende all'infinito.  

# Risposta all'impulso  

Si vuole ora esaminare la risposta del sistema all'impulso unitario $v_{in} = \delta(t)$.  

$V_{L}(s) = G(s) \cdot V_{in}(s)$  

E' dimostrabile che la trasformata dell'impulso unitario equivale a $\delta(s) = 1$ per cui...  

$V_{L}(s) = G(s) \cdot 1 = \dfrac{s}{5+s} = s \cdot \dfrac{1}{5+s}$  

Sapendo che $s \cdot F(s)$ e' una derivata otteniamo infine che...  

$v_{L}(t) = \dfrac{\Delta e^{-5t}\cdot u(t)}{\Delta t}$  

![impulse_response](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/58425d8b-2e2c-45fb-9a74-5407cf0d6e7f)  

Si nota allora come la risposta del sistema all'impulso, al contrario del gradino unitario, dipenda unicamente dalla composizione del sistema stesso, ovvero da $G(s)$. Inoltre, e' importante notare come la risposta cambi singnificativamente in dipendenza del tipo di segnale in ingresso.  
