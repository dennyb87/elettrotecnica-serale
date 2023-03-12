# Scomposizione trinomio di secondo grado  

Consideriamo un trinomio nella forma:  

$ax^2 + bx + c$  

Se troviamo due numeri reali $p$ ed $s$ tali che:  

$p + s = b$  
$p \cdot s = a \cdot c$  

Possiamo allora scomporre il trinomio come segue:  

$ax^2 + bx + c = a\biggl(x + \dfrac{s}{a}\biggr) \biggl(x + \dfrac{p}{a}\biggr)$  

Vediamo un esempio...  

$2x^2 + (-2-5)x + 5$  

Sapendo quindi che $p \cdot s = a \cdot c = 2 \cdot 5 = 10$ vogliamo trovare $p + s = -7$ a tentativi individuando quindi i divisori di $10$ il cui prodotto sia $10$ e la somma $-7$.  

|       |      |              |
| ----- | ---- | ------------ |
| $+10$ | $+1$ | $\times$     |
| $+10$ | $-1$ | $\times$     |
| ...   | ...  | ...          |
| $+5$  | $-2$ | $\times$     |
| $-5$  | $-2$ | $\checkmark$ |

Abbiamo allora trovato $p = -2$ ed $s = -5$ possiamo ora riscrivere l'espressione.  

$2x^2 - 7x + 5$  
$2x^2 + (-2-5)x + 5$  
$2x^2 -2x -5x + 5$  
$2x(x - 1) - 5(x - 1)$  
$(x - 1)(2x - 5)$  

## Trinomio speciale  

Nel caso speciale in cui $a = 1$ si ha che $p \cdot s = 1 \cdot c = c$ allora possiamo scrivere:  

$x^2 + (p + s)x + (p \cdot s)$  
$x^2 + px + sx + ps$  
$x(x + s) + p(x + s)$  
$(x + s)(x + p)$  
 

## Soluzione attraverso le radici dell'equazione di secondo grado    

Il metodo piu' generico che funziona per ogni trinomio e' appunto quello di utilizzare la formula per la risoluzione delle equazioni di secondo grado per trovare le radici ed utilizzarle per la scomposizione. Una volta ottenute le soluzioni $x_1, x_2$ potranno essere utilizzate per la scomposizione come segue:  

$ax^2 + bx + c = a(x - x_1)(x - x_2)$  

Si noti che questa formulazione e' del tutto analoga a quella vista precedentemente.    

$ax^2 + bx + c = a\biggl(x + \dfrac{s}{a}\biggr) \biggl(x + \dfrac{p}{a}\biggr)$  

Formuliamo allora l'equazione:  

$ax^2 + bx + c = 0$  