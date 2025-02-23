# Derivata di una potenza  

La derivata e' quindi il limite del rappporto incrementale, ovvero la pendenza della retta tangente alla funzione in un certo punto. Questa puo' essere espressa in notazioni diverse, tra cui:  

$$
\begin{aligned}
    \dfrac{df}{dx}\bigg|_{x=x_0}\\
    \\
    Df(x_0)\\
    \\
    f^\prime(x_0)\\
\end{aligned}
$$  

Data una funzione $f(x) = x^2$ si vuole calcolare $f^\prime(x_0)$ dove $x_0 = 2$ quindi dalla definizione...   

$$
\begin{aligned}
    f^\prime(x) &= \displaystyle{\lim_{h \to 0}\ \dfrac{f(x+h)-f(x)}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{f(2+h)-f(2)}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{(2+h)^2-(2)^2}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{\cancel{4}+h^2+4h-\cancel{4}}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ h+4} = 4
\end{aligned}
$$

## Teorema della potenza  

Il teorema della potenza ci permette di calcolare la derivata di funzioni del tipo $f(x) = x^n$ in modo piu' rapido. In particolare si puo' dimostrare che...  

$f(x) = x^n \implies f^\prime(x) = nx^{n-1}$  

Una semplice dimostrazione e' possible assumendo $x \ne 0$  

$$
\begin{aligned}
    f^\prime(x) &= \displaystyle{\lim_{h \to 0}\ \dfrac{f(x+h)-f(x)}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{(x+h)^n-x^n}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{\bigg[x\cdot\bigg(1+\dfrac{h}{x}\bigg)\bigg]^n-x^n}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \dfrac{x^n\cdot\bigg(1+\dfrac{h}{x}\bigg)^n-x^n}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ x^n\cdot\dfrac{\bigg(1+\dfrac{h}{x}\bigg)^n-1}{h}}\\
    \\
    &=\displaystyle{\lim_{h \to 0}\ \underbrace{x^n\cdot\dfrac{1}{x}}_{x^{n-1}}\cdot\dfrac{\bigg(1+\dfrac{h}{x}\bigg)^n-1}{\dfrac{h}{x}}} = nx^{n-1}\\
    \\
\end{aligned}
$$  

Nell'ultimo passaggio moltiplichiamo e dividamo per $\dfrac{1}{x}$ utilizzando il limite notevole che permette di ridurre il termine a destra ad $n$  

$\displaystyle{\lim_{x \to 0}\ \dfrac{(1+x)^k-1}{x}} = k$  
