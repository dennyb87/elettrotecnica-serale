# Studio di funzione  

Lo studio di funzione ci permette di ricavare il comportamento di una funzione e tracciarne quindi il grafico qualitativo partendo dalla sua espressione analitica. In particolare si evidenziano i seguenti passaggi:

1. dominio
2. simmetrie
3. zeri
4. segno
5. comportamento agli estremi
6. derivata prima

Vogliamo eseguire lo studio di funzione di:  

$y = \dfrac{x^3}{(x-1)^2}$  

## Dominio  

Il numeratore non da' problemi per cui si esamina solo il denominatore.  

$(x-1)^2 \ne 0 \implies x\ne 1$  

Allora il dominio sara'...  

$D:(-\infty,1) \cup (1,+\infty)$  

## Simmetrie  

Ricordando che una funzione e' pari quando $f(x) = f(-x)$  

$f(-x) = \dfrac{-x^3}{(-x-1)^2}$  

Si ha allora che $f(x) \ne f(-x)$ percio' non e' pari! Inoltre ricordando che una funzione e' dispari quando $f(-x) = -f(x)$  

$-f(x) = \dfrac{-x^3}{(x-1)^2}$  

Dato che $f(-x) \ne -f(x)$ non e' nemmeno dispari, ovvero non ci sono simmetrie!  

## Zeri  

Troviamo l'intersezione con l'asse $x$  

$y = 0 \implies \dfrac{x^3}{(x-1)^2} = 0$  

Ma l'equazione diventa un'identita' solo quando il numeratore e' zero, ovvero quando $x = 0$ percio' si ha un punto di intersezione con l'asse $x$ in $P_1 = (0, 0)$  

Troviamo ora l'intersezione con l'asse $y$  

$x = 0 \implies y = \dfrac{0^3}{(0-1)^2} = 0$  

Si ha allora un punto di intersezione $P_2$ che coincide con $P_1$  

$P_2 \equiv P_1 = (0, 0)$  

## Segno  

Vogliamo sapere quando $y$ e' positiva percio' poniamo $y > 0$  

$\dfrac{x^3}{(x-1)^2} > 0$  

Tenendo conto del **dominio** $x \ne 1$ il denominatore e' sempre positivo data la potenza pari, mentre a causa della potenza dispari il numeratore e' positivo solo quando $x$ e' positiva.  

Allora $y$ e' positiva quando $x > 0\ \land \ x \ne 1$  

## Comportamenti agli estremi  

Vogliamo esaminare il comportamento della funzione agli estremi degli intervalli del dominio $D:(-\infty,1) \cup (1,+\infty)$  
 
$\displaystyle{\lim_{x\to -\infty}}\ \dfrac{x^3}{(x-1)^2} = \dfrac{x^3}{x^2} = x = -\infty$  

$\displaystyle{\lim_{x\to 1^-}}\ \dfrac{x^3}{(x-1)^2} = \dfrac{1}{(1^--1)^2} = \dfrac{1}{0^+} = +\infty$  

$\displaystyle{\lim_{x\to 1^+}}\ \dfrac{x^3}{(x-1)^2} = \dfrac{1}{(1^+-1)^2} = \dfrac{1}{0^+} = +\infty$  

$\displaystyle{\lim_{x\to +\infty}}\ \dfrac{x^3}{(x-1)^2} = \dfrac{x^3}{x^2} = x = +\infty$  

Non si hanno asintoti orizzontali poiche' quando $x \to \pm\infty$ la funzione tende all'infinito. Andiamo allora alla ricerca di asintoti obliqui.  

$m = \displaystyle{\lim_{x\to \pm\infty}}\ \dfrac{x^3}{(x-1)^2}\cdot \dfrac{1}{x} = \dfrac{x^3}{x^3} = 1$  

$c = \displaystyle{\lim_{x\to \pm\infty}}\ \dfrac{x^3}{(x-1)^2}-x = \dfrac{x^3-x(x-1)^2}{(x-1)^2} = \dfrac{2x^2-x}{(x-1)^2} = \dfrac{2x^2}{x^2} = 2$  

Si ha allora un asintoto obliquo di equazione $y = x+2$  

## Derivata prima  

Ricordando la derivata del quoziente...   

$D\ \dfrac{f(x)}{g(x)} = \dfrac{f^\prime(x)\cdot g(x)-f(x)\cdot g^\prime(x)}{[g(x)]^2}$  

$y^\prime = \dfrac{3x^2(x-1)-2x^3(x-1)}{(x-1)^4} = \dfrac{x^2\bigg[3(x-1)-2x\bigg]}{(x-1)^3} = \dfrac{x^2(3x-2x-3)}{(x-1)^3}$  

$y^\prime = \dfrac{x^2(x-3)}{(x-1)^3}$  

## Grafico  

![graph_function](https://github.com/user-attachments/assets/78d34c30-642a-4027-a785-bd310ac4d612)  
