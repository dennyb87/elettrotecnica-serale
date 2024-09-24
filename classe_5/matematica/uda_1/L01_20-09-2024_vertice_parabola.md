# Vertice di una parabola  

Le equazioni di secondo grado geometricamente rappresentano delle parabole. Esaminando casi semplici si puo' intuire come $c$ contribuisca esclusivamente allo spostamento verticale.  

![parabola_shifts](https://github.com/user-attachments/assets/e71f3ce2-7d29-4668-83a3-512103dd498a)  

Con $y = x^2$ si ha che il vertice si trova all'origine quando $x = 0$ e cosi' via...  

## La coordinata x del vertice  

Si vuole ora riscrivere $y = (x-2)^2-1$ espandendo il quadrato di binomio arrivando alla forma $y = ax^2+bx+c$  

$y = x^2-4x+3$  

Sappiamo pero' che la coordinata x del vertice non e' influenzata dallo spostamento verticale, per cui possiamo ignorare $c$ a tutti gli effetti esaminando una parabola simile.  

$y = ax^2+bx$  

![vertex_01](https://github.com/user-attachments/assets/a05ea1bb-3d64-40b2-88af-91d26b22cbbb)  

Scomponendo otteniamo...  

$y = x(ax + b)$  

Si nota immediatamente che questa nuova parabola interseca l'asse delle ascisse quando $x = 0$ oppure $x = -\dfrac{b}{a}$ e questo implica che la coordinata $V_x$ del vertice deve essere a meta' tra questi due valori, ovvero:  

$V_x = -\dfrac{b}{2a}$  

Sostiuendo i valori dell'equazione originale otteniamo infine...  

$V_x = -\dfrac{b}{2a} = -\bigg(\dfrac{-4}{2}\bigg) = 2$


## La coordinata y del vertice  

Dato il classico trinomio di secondo grado:  

$y = ax^2+bx+c$  

Si vuole completarne il quadrato...  

$y = a\bigg(x^2+\dfrac{b}{a}x\bigg)+c$  

$y = a\bigg[\bigg(x+\dfrac{b}{2a}\bigg)^2 -\dfrac{b^2}{4a^2}\bigg]+c$  

$y = a\bigg(x+\dfrac{b}{2a}\bigg)^2-\dfrac{b^2}{4a}+c$  

$y = a\bigg(x+\dfrac{b}{2a}\bigg)^2 + \dfrac{4ac -b^2}{4a}$  

A questo punto e' importante notare che quando $x = V_x = -\dfrac{b}{2a}$ si ha che il primo termine diventa zero, e il termine restante rappresenta quindi il valore minimo possible di $y$ ovvero la coordinata $V_y$ del vertice. Riarrangiando scopriamo infine che...  

$V_y = \dfrac{4ac -b^2}{4a} = \dfrac{-(b^2-4ac)}{4a} =-\dfrac{\Delta}{4a}$  


In generale...  


$V = (V_x,V_y) = \bigg(-\dfrac{b}{2a},\ -\dfrac{\Delta}{4a}\bigg)$
