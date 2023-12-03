# Forme canoniche  

Per poter definire la **forma canonica** dobbia prima definire i concetti di **mintermini** e **maxtermini**.  

## Mintermine  

Un mintermine e' il prodotto logico degli input, negati o non negati, per cui l'output equivale ad $1$.  

## Maxtermine  

Un maxtermine e' la somma logica degli input, negati o non negati, per cui l'output equivale ad $0$.  

| A   | B   | Y   | minterms        | maxterms         |
| --- | --- | --- | --------------- | ---------------- |
| 0   | 0   | 0   |                 | $A+B$            |
| 0   | 1   | 0   |                 | $A+\overline{B}$ |
| 1   | 0   | 1   | $A\overline{B}$ |                  |
| 1   | 1   | 1   | $A \cdot B$     |                  |

In questo esempio e' possibile quindi esprimere $y$ in due modi:  

* come prodotto di maxtermini $y = (A+B) \cdot (A+\overline{B})$
* come somma di mintermini $y = A\overline{B} + AB$

Queste sono appunto chiamate: **forma canonica del prodotto** e **forma canonica della somma**, ovvero l'espressione di $y$ come sommatoria di mintermini o come prodotto di maxtermini.  

$\sum_{i=0}^n m_i = m_0 + m_1 + ... + m_n$  

$\prod_{i=0}^n M_i = M_0 \cdot M_1 \cdot ... \cdot M_n$  

E' importante notare che la forma canonica non equivale necessariamente alla forma minima, infatti semplificando le forme canoniche nel nostro esempio otterremmo facilmente:  

$y = A$  
