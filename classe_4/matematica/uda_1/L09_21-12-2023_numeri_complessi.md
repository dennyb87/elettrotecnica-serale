# Numeri complessi  

![number_sets_venn_diagram](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/21065536-4eba-4002-82c5-bb03ea078ed0)  

I numeri complessi nascono dall'esigenza di estendere l'insieme dei numeri reali, per permettere operazioni per le quali non sarebbe altrimenti ammessa soluzione. Prendiamo ad esempio l'equazione:  

$x^2 + 1 = 0 \implies x^2 = -1$  

In $\mathbb{R}$ non esiste un numero che moltiplicato per se stesso dia come risultato $-1$. E' necessario allora estendere $\mathbb{R}$ definendo l'insieme dei numeri complessi $\mathbb{C}$, si introduce cosi' l'unita' immaginaria $i$ ovvero:  

$i \coloneqq \sqrt{-1}$  

## Interpretazione geometrica  

Un numero complesso $z$ e' allora un numero composto da una parte reale $a$ ed una parte immaginaria $ib$:  

$z = a + ib$  

Geometricamente e' possibile rappresentare questi numeri in un piano simile a quello cartesiano, detto piano di Gauss (o piano complesso). Questo avra' un asse reale, ed uno immaginario.  

![complex_plane](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/2939aa7d-a40f-415e-b2a3-84d1b77d24f5)  


Il numero complesso $z$ puo' essere allora visto come una somma vettoriale $\vec{a} + \vec{i} \cdot \vec{b}$ dove $\vec{i} = (0, 1)$ e' il vettore immaginario unitario:  

$z = a + ib = (a, 0) + (0, 1) \cdot (b, 0)$  

Se $(a, 0)$ non ha parte immaginaria possiamo scrivere semplicemente $a$ mentre...  

$ib = (0, 1) \cdot (b, 0) = (0 + i) \cdot (b + i0) = 0b + i0 + ib + i^20 = ib$  

Risolvendo algebricamente si puo' notare che la parte reale scompare diventanto puramente immaginaria, l'equivalente geometrico di una rotazione di $90^\circ$.  

![complex_rotation_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cc1d5c72-1d5e-4b35-95db-d15334c87162)  

## Moltiplicazione  

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

In particolare, moltiplicare per $i$ causa rotazioni $90^\circ$ in senso antiorario.  

![i_rotations](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/3cd89d72-87e1-4a82-ba16-cf644d30ac0b)  

Va da se che per semplificare espressioni di questo tipo $i^{13}$ e' sufficiente dividere l'esponente per $4$ utilizzando il resto come nuovo esponente.  

$i^{12} = i^0 = 1$  
$i^{13} = i^{1} = i$  
$i^{14} = i^2 = -1$  
$i^{15} = i^3 = -i$  

## Somma  

La somma di due numeri complessi equivale allora ad una somma vettoriale:  

$z_1 + z_2 = (a, b) + (c, d) = (a + c, b + d)$  

## Divisione  

La divisione si esegue semplicemente moltiplicando per l'inverso del numero per cui si vuole dividere.  

$\dfrac{z_1}{z_2} = z_1 \cdot \dfrac{1}{z_2}$  

Con $z_2 = a + ib$ si ha allora che...  

$\dfrac{1}{z_2} = \dfrac{1}{a + ib}$  

Per semplicita' si vuole rimuovere la parte immaginaria al denominatore (moltiplicando per il coniugato):  

$\dfrac{1}{z_2} = \dfrac{1}{a + ib} \cdot \dfrac{a - ib}{a - ib} = \dfrac{a - ib}{a^2 - (ib)^2} = \dfrac{a - ib}{a^2 + b^2}$  

Si ha infine...  

$\dfrac{z_1}{z_2} = z_1 \cdot \dfrac{a - ib}{a^2 + b^2}$  

## Complesso coniugato  

![complesso_coniugato](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9fec01bf-94f7-4b83-8303-9a8b5267ea6c)  

Il coniugio di un numero complesso $z$ e' quel numero complesso $\overline{z}$ che ha parte reale uguale al primo, ma parte immaginaria di segno opposto.  

$z = a + ib$  
$\overline{z} = a - ib$  

