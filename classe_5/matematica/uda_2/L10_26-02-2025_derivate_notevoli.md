# Derivate notevoli  


|               |                          |                             |
| ------------- | ------------------------ | --------------------------- |
| $D\ c$        | $0$                      | $\forall\ c \in \mathbb{R}$ |
| $D\ x^n$      | $nx^{n-1}$               | $\forall\ n \in \mathbb{N}$ |
| $D\ \sin x$   | $\cos x$                 |                             |
| $D\ \cos x$   | $-\sin x$                |                             |
| $D\ a^x$      | $a^x\cdot\ln a$          |                             |
| $D\ e^x$      | $e^x$                    |                             |
| $D\ \log_a x$ | $\dfrac{1}{x\cdot\ln a}$ |                             |
| $D\ \ln x$    | $\dfrac{1}{x}$           |                             |


# Teoremi di derivazione  

|           |                                 |                                                                 |
| --------- | ------------------------------- | --------------------------------------------------------------- |
| costante  | $D\ c\cdot f(x)$                | $c \cdot f^\prime(x)$                                           |
| somma     | $D\ \bigg[f(x)+g(x)\bigg]$      | $f^\prime(x)+g^\prime(x)$                                       |
| prodotto  | $D\ \bigg[f(x)\cdot g(x)\bigg]$ | $f^\prime(x)\cdot g(x)+f(x)\cdot g^\prime(x)$                   |
| quoziente | $D\ \dfrac{f(x)}{g(x)}$         | $\dfrac{f^\prime(x)\cdot g(x)-f(x)\cdot g^\prime(x)}{[g(x)]^2}$ |
| reciproca | $D\ \dfrac{1}{f(x)}$            | $\dfrac{f^\prime(x)}{[f(x)]^2}$                                 |
| composta  | $D\ f(g(x))$                    | $f^\prime(g(x))\cdot g^\prime(x)$                               |

## Esercizio 1  

$h(x) = f(x)\cdot g(x) = (3x^2-1)\cdot(2x^2+5)$  

$f^\prime(x) = 6x$  
$g^\prime(x) = 4x$  

Allora per il teorema del prodotto...  

$h^\prime(x) = 6x(2x^2+5)+4x(3x^2-1)$  

$h^\prime(x) = 12x^3+30x+12x^3-4x = 24x^3+26x$  


## Esercizio 2    

$h(x) = \dfrac{f(x)}{g(x)} =\dfrac{x^3\cdot(x-1)^4}{(x+2)^2}$  

Per il teorema del prodotto al numeratore si ha che...  

$f^\prime (x) = 3x^2\cdot(x-1)^4+4(x-1)^3\cdot x^3$  

Allora per il teorema del quoziente...  

$h^\prime(x) = \dfrac{\bigg[3x^2\cdot(x-1)^4+4(x-1)^3\cdot x^3\bigg]\cdot (x+2)^2-2(x+2)\cdot x^3(x-1)^4}{[(x+2)^2]^2}$  

$h^\prime(x) = \dfrac{\bigg[3x^2\cdot(x-1)^4+4(x-1)^3\cdot x^3\bigg]\cdot (x+2)-2x^3(x-1)^4}{(x+2)^3}$  

$h^\prime(x) = \dfrac{x^2(x-1)^3\bigg[3(x-1)+4x\bigg]\cdot (x+2)-2x^3(x-1)^4}{(x+2)^3}$  

$h^\prime(x) = \dfrac{x^2(x-1)^3\bigg(\bigg[3(x-1)+4x\bigg]\cdot (x+2)-2x(x-1)\bigg)}{(x+2)^3}$  

$h^\prime(x) = \dfrac{x^2(x-1)^3\bigg(\bigg[3x-3+4x\bigg]\cdot (x+2)-2x^2+2x\bigg)}{(x+2)^3}$  

$h^\prime(x) = \dfrac{x^2(x-1)^3\bigg(3x^2+6x-3x-6+4x^2+8x-2x^2+2x\bigg)}{(x+2)^3}$  

$h^\prime(x) = \dfrac{x^2(x-1)^3\bigg(5x^2+13x-6\bigg)}{(x+2)^3}$  

