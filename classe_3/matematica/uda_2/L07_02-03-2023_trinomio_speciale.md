# Trinomio speciale  

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

Nel caso speciale in cui $a = 1$ si ha che $p \cdot s = 1 \cdot c = c$ allora possiamo scrivere:  

$x^2 + (p + s)x + (p \cdot s)$  
$x^2 + px + sx + ps$  
$x(x + s) + p(x + s)$  
$(x + s)(x + p)$  