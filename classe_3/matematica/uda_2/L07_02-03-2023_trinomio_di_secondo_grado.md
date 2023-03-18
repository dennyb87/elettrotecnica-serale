# Scomposizione trinomio di secondo grado  

Consideriamo un trinomio nella forma:  

$ax^2 + bx + c$  

Se troviamo due numeri reali $p$ ed $s$ tali che:  

$p + s = b$  
$p \cdot s = a \cdot c$  

Possiamo allora scomporre il trinomio come segue:  

$ax^2 + bx + c = a\bigg(x + \dfrac{s}{a}\bigg) \bigg(x + \dfrac{p}{a}\bigg)$  

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
 

## Scomposizione attraverso le radici dell'equazione di secondo grado  

Un metodo generico che funziona per ogni trinomio e' appunto quello di utilizzare la formula per la risoluzione delle equazioni di secondo grado per trovare le radici ed utilizzarle per la scomposizione. Una volta ottenute le soluzioni $x_1,\ x_2$ potranno essere utilizzate per la scomposizione come segue:  

$ax^2 + bx + c = a(x - x_1)(x - x_2)$  

Si noti che questa formulazione e' del tutto analoga a quella vista precedentemente:  

$ax^2 + bx + c = a\bigg(x + \dfrac{s}{a}\bigg) \bigg(x + \dfrac{p}{a}\bigg)$  

Deriviamo ora la formula di risoluzione generale dell'equazione:  

$ax^2 + bx + c = 0$  

$\cancel{a}x^2 + \dfrac{b}{a}x + \dfrac{c}{a} = 0$  

$x^2 + \dfrac{b}{a}x = - \dfrac{c}{a}$  

Adesso e' importante notare che geometricamente si ha un quadrato incompleto, e si vuole percio' *completare il quadrato* aggiungendo $\dfrac{b^2}{4a^2}$ (parte arancione in figura) passaggio che ci permette di semplificare il termine di sinistra in un quadrado di binomio.  

![completing_the_square](https://user-images.githubusercontent.com/7195133/224638542-8126aaf5-6a56-46bc-bb35-848f0c9acbac.jpg)  

$x^2 + \dfrac{b}{a}x = - \dfrac{c}{a}$  

$x^2 + \dfrac{b}{a}x + \dfrac{b^2}{4a^2} = - \dfrac{c}{a} + \dfrac{b^2}{4a^2}$  

$\bigg(x + \dfrac{b}{2a}\bigg)^2 = \dfrac{b^2 - 4ac}{4a^2}$  

$\bigg(x + \dfrac{b}{2a}\bigg)^2 = \dfrac{b^2 - 4ac}{4a^2}$  

$x + \dfrac{b}{2a} = \pm \dfrac{\sqrt{b^2 - 4ac}}{2a}$  

$x = \dfrac{-b \pm\sqrt{b^2 - 4ac}}{2a}$  

La quantita' sotto radice puo' essere positiva o negativa, cio' significa che si possono avere due soluzioni $x_1,\ x_2$ che come abbiamo visto si possono utilizzare per la scomposizione:  

$ax^2 + bx + c = a(x - x_1)(x - x_2)$  

Supponiamo allora di voler scomporre il polinomio $2x^2 - x -1$ ricordandoci che per poterlo riscrivere nella forma $a(x - x_1)(x - x_2)$ ci bastera' trovare le soluzioni $x_1,\ x_2$ grazie alla formula che abbiamo appena derivato.  

$\dfrac{-b \pm\sqrt{b^2 - 4ac}}{2a} = \dfrac{-(-1) \pm\sqrt{(-1)^2 - 4 \cdot 2 \cdot (- 1)}}{2 \cdot 2} = \dfrac{1 \pm\sqrt{9}}{4} = \dfrac{1\pm 3}{4}$  

$x_1 = \dfrac{1 + 3}{4} = 1$  

$x_2 = -\dfrac{1 - 3}{4} = - \dfrac{1}{2}$  

Trovate le soluzioni possiamo allora usarle per scomporre il polinomio.  

$2x^2 - x - 1 = 2(x - 1)(x + \frac{1}{2})$  