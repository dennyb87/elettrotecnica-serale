# Filtro passa-alto  

![high_pass_filter](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/998ff4ce-cf32-4560-a151-35b783535a62)  

Prendiamo delle grandezze arbitrarie per ricavare l'andamento della corrente nel caso limite di un generatore in continua.  

$R = 2\ \Omega$  
$L = 0.5\ H$  
$e(t) = 20 \cdot u(t) \implies E(s) = \dfrac{20}{s}$  

$I(s) = \dfrac{E(s)}{Z_{tot}} = \dfrac{20}{s} \cdot \dfrac{1}{R+Ls} = \dfrac{20}{s} \cdot \dfrac{1}{2+0.5s}$  

$I(s) = \dfrac{20}{s} \cdot \dfrac{1}{0.5(s+4)} = \dfrac{20}{0.5} \cdot \dfrac{1}{s(s+4)} = 40 \cdot \dfrac{1}{s(s+4)}$  

$i(t) = 40 \cdot \dfrac{1}{a}\bigg(1-e^{-at}\bigg) \cdot u(t) = 10- 10e^{-4t} \cdot u(t)$  

![current_graph_high_pass_filter](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/adec92a0-accd-4498-b174-4dd2545ac257)  

All'accensione la corrente parta da zero ma la sua variazione ai primi istanti e' massima! Questo e' ancora piu' evidente mano che ci si avvicina allo zero...  

![zoomedin_graph_current_at_zero](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/79a1ae1c-f20b-44b4-8433-aa365c838fc1)  

Valutando in modo approssimativo $v(t)$ dove $t \simeq 0$ scopriamo che...  

$v(t) = L\dfrac{\Delta i}{\Delta t} = 0.5 \cdot \dfrac{0.0004 - 0}{0.00001 - 0} = 20\ V$  

Si ha allora che all'accensione del generatore la caduta di tensione su $R$ e' zero.  

$i(0^+) \simeq 0$  

$V_R = R \cdot i(0^+) = R \cdot 0 = 0$  

Nonostante la corrente sia $\simeq 0$ dato che sta crescendo la sua variazione e' massima, per cui $X_L$ e' al suo massimo e tutta la tensione cade ha appunto su $L$. Quando il sistema e' a regime, non si ha piu' variazione di corrente e' l'induttore diventa un cortocircuito, e di conseguenza si ha zero caduta di tensione su $L$  

$v_L(t)\vert_{t=\infty} = X_L \cdot i(t) = 0 \cdot i(t) = 0$  

## Tabella all'aumentare della frequenza  

| $f[Hz]$ | $V_{in}[V]$ | $V_{out}[V]$ | $G$  |
| ------- | ----------- | ------------ | ---- |
| 0       | 20          | 0            | 0    |
| 0.1     | 20          | 3            | 0.15 |
| 0.5     | 20          | 12           | 0.6  |

Di seguito i grafici delle righe in tabella. 

![high_pass_filter_0Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/83170ee3-66c1-48d3-b118-9aebbacbed59)  

![high_pass_filter_0 1Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/5261afbd-b545-4663-974c-216bd2e2006e)  

![high_pass_filter_0 5Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cea9e85b-f5aa-4ed7-bf34-9775242d43b4)  

In modo analogo al filtro passa-basso in quello passa-alto si ha una caratteristica di questo tipo.  

![high_pass_filter_characteristic](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cb9e29b2-63dc-4aff-8bdc-aa14849aece7)  

$G(s) = \dfrac{Ls}{R+Ls} = \dfrac{0.5s}{2+0.5s} = \dfrac{\cancel{0.5}s}{\cancel{0.5}(s+4)} = s \cdot \dfrac{1}{s+4}$  

Per le proprieta' della trasformata di Laplace si ha che la funzione di trasferimento del filtro passa-alto non e' altro che la derivata della funzione di trasferimento del filtro passa-basso.  

$s \cdot F(s) \implies \dfrac{\Delta f(t)}{\Delta t}$  

$s \cdot \dfrac{1}{s+4} \implies \dfrac{\Delta e^{-4t} \cdot u(t)}{\Delta t}$  

Quando $\omega = a_G = 4\ \frac{rad}{s}$ si ha la frequenza di taglio, *cut-off frequency* $f_c$ in questo caso $f_c = \dfrac{a_G}{2\pi} = \dfrac{4}{2\pi} \simeq 0.64\ Hz$ dove $G = \dfrac{1}{\sqrt{2}}$ e lascia passare gran parte del segnale.  
