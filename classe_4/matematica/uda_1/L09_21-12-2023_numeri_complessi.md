# Numeri complessi  

I numeri complessi, o immaginari, nascono dall'esigenza di estendere l'insieme dei numeri reali, per permettere operazioni per le quali non sarebbe altrimenti ammessa soluzione. Prendiamo ad esempio l'equazione:  

$x^2 + 1 = 0 \implies x^2 = -1$  

In $\mathbb{R}$ non esiste un numero che moltiplicato per se stesso dia come risultato $-1$. E' necessario allora estendere $\mathbb{R}$ definendo l'insieme dei numeri complessi $\mathbb{C}$, si introduce cosi' l'unita' immaginaria $i$ ovvero:  

$i \coloneqq \sqrt{-1}$  

Un numero complesso $z$ e' allora un numero composto da una parte reale $a$ ed una parte immaginaria $ib$:  

$z = a + ib$  

Geometricamente e' possibile rappresentare questi numeri in un piano simile a quello cartesiano, detto piano di Gauss (o piano complesso). Questo avra' un asse reale, ed uno immaginario.  

![complex_plane](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/2939aa7d-a40f-415e-b2a3-84d1b77d24f5)  

Il numero complesso $z$ puo' essere allora visto come una somma vettoriale $a + ib$ dove $b$ viene moltiplicato per il vettore immaginario unitario $i = (0, 1)$ ovvero...  

$z = (a, 0) + (0, 1) \cdot (b, 0)$  

Se $(a, 0)$ non ha parte immaginaria possiamo scrivere semplicemente $a$ mentre...  

$(0, 1) \cdot (b, 0) = (0 + i) \cdot (b + i0) = 0b + i0 + ib + i^20 = ib$  

Risolvendo algebricamente si puo' notare che la parte reale scompare diventanto puramente immaginaria, l'equivalente geometrico di una rotazione di $90^\circ$.  

![complex_rotation_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cc1d5c72-1d5e-4b35-95db-d15334c87162)  

Generalizzando possiamo descrivere la moltiplicazione tra due numeri complessi come segue:  

$z_1 = a + ib$  
$z_2 = c + id$  

$z_1 \cdot z_2 = (a + ib) \cdot (c + id) = ac + iad + ibc + i^2bd$  

Ma $i^2 = -1$ percio'...  

$z_1 \cdot z_2 = ac - bd + i (ad + bc)$  

L'equivalente della coppia ordinata:  

$z_1 \cdot z_2 = (ac - bd, ad + bc)$  

![complex_rotation_02](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/42a160c1-0efb-408e-9b8b-09fb9fdd7b3b)  

$z = (4 +3i)$  

$iz = i(4 + 3i) = 4i + 3i^2 = 4i + 3 \cdot -1 = -3 + 4i$  
