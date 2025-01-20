# Asintoti obliqui  

![slope](https://github.com/user-attachments/assets/60e7ce04-e1d5-4687-88eb-77e206d99891)  

Sappiamo che l'asintoto verticale si trova valutando il limite della funzione con $x \to x_0$ mentre quello orizzontale con $x \to \pm\infty$. Nel caso in cui l'asintoto orizzontale non esistesse, potremmo essere di fronte ad un **asintoto obliquo**, questo e' appunto una retta ne' orizzontale ne' verticale, che avra' quindi pendenza diversa da zero.  

$y = mx+c$  

Questa retta puo' essere derivata utilizzando proprio la sua definizione e valutando i limiti per ricavare $m$ e $c$...  

$\displaystyle{\lim_{x \to \pm\infty}}\ \dfrac{f(x)}{x} = m$  

$\displaystyle{\lim_{x \to \pm\infty}}\ \bigg(f(x) - mx\bigg) = c$  

## Esempio  

$y = \dfrac{x^3+1}{x^2+2x}$  

Troviamo il dominio...  

$y = \dfrac{x^3+1}{x^2+2x} = \dfrac{x^3+1}{x(x+2)} \implies D: \mathbb{R} -\lbrace 0;-2\rbrace$  

Si hanno quindi due asintoti verticali che per brevita' non andremo a valutare. Valutiamo invece quelli orizzontali:  

$\displaystyle{\lim_{x \to \pm\infty}}\ \dfrac{x^3+1}{x^2+2x} = \dfrac{x^3\bigg(1+\dfrac{1}{x^3}\bigg)}{x^2\bigg(1+\dfrac{2}{x}\bigg)} = \dfrac{x}{1} = \pm\infty$  

Il limite non esiste percio' non si hanno asintoti orizzontali. Procediamo alla ricerca degli asintoti obliqui.  

$\displaystyle{\lim_{x \to \pm\infty}}\ \dfrac{f(x)}{x} = \dfrac{x^3+1}{x^2+2x}\cdot\dfrac{1}{x} = \dfrac{x}{1}\cdot\dfrac{1}{x} = 1 \implies m = 1$  

$\displaystyle{\lim_{x \to \pm\infty}}\ \bigg(f(x) - mx\bigg) = \dfrac{x^3+1}{x^2+2x} -x = \dfrac{\cancel{x^3}+1-\cancel{x^3}-2x^2)}{x^2+2x} = \dfrac{\cancel{x^2}\bigg(\dfrac{1}{x^2}-2\bigg)}{\cancel{x^2}\bigg(1+\dfrac{2}{x}\bigg)} = -2 \implies c = -2$  

Si ha allora un asintoto obliquo con equazione $y = x-2$  

![asintoto_obliquo](https://github.com/user-attachments/assets/347efad7-d346-4d25-9bff-e5d180d29403)  
