# Introduzione alle forme indeterminate  

## Quoziente  

Consideriamo il limite...  

$\displaystyle{\lim_{x\to +\infty}}\ \dfrac{x^3}{\log x}$  

In questo caso sia il numeratore che il denominatore tendono a infinito ottenendo $\dfrac{\infty}{\infty}$ ma questa e' una forma indeterminata in quanto non e' possibile decidere quale sia il risultato. Conoscendo l'algebra degli infiniti sappiamo che:  

$\infty \cdot 5 = \infty$  
$\infty \cdot 6 = \infty$  

Ma questo implicherebbe che $5 = \dfrac{\infty}{\infty} = 6$ e cio' non e' possibile quindi dimostrando la sua natura indeterminata!  

![infinity_rate](https://github.com/user-attachments/assets/9fe62e8d-6f5b-4580-9668-20114e1db7ce)  

Per risolvere questo tipo di forma indeterminata si deve allora esaminare il grafico delle funzioni oggetto della frazione. In particolare si puo' notare che le due funzioni tendono a infinito a velocita' diverse. In questo caso $x^3$ tende ad infinito molto piu' velocemente, percio' possiamo considerare $\log x = 1$ o un qualunque altro numero reale positivo.  

Si ha infine che...  

$\displaystyle{\lim_{x\to +\infty}}\ \dfrac{x^3}{\log x} = \dfrac{+\infty}{1} = +\infty$  


## Somma  

Consideriamo il limite...  

$\displaystyle{\lim_{x\to -\infty}} (4x^2-2x+3) = (4(-\infty)^2-2\infty+\cancel{3}) = +\infty-\infty$  

Intuitivamente, almeno dal punto di vista dell'algebra degli infiniti, verrebbe da pensare che $+\infty-\infty = 0$ ma cio' porterebbe a una contraddizione....  

$+\infty-\infty = 0$  
$+\infty-\infty+1 = 0+1$  

Ma allora $+\infty-\infty = 1$ e questo non e' possible! Per cui $+\infty-\infty$ e' considerata una forma indeterminata. L'agebra degli infiniti pero' a mio parere nasconde cosa stia realmente accadendo...  

$\displaystyle{\lim_{x\to -\infty}} (4x^2-2x+3)$  

Se ignoriamo la costante $3$ che non aggiunge informazione, notiamo che siamo di fronte a due funzioni:  

$f(x) = 4x^2$  
$g(x) = -2x$  

![limits_intuition](https://github.com/user-attachments/assets/113bf331-dd3f-41d3-bff5-ae41a2067800)  

Esaminando il grafico delle funzioni separatamente notiamo proprio che $4x^2 \to +\infty$ mentre $-2x \to -\infty$ rendendo poco chiara la tendenza della loro somma. Dal grafico possiamo intuire che $f(x)$ tende a $+\infty$ piu' velocemente rispetto a $g(x)\to-\infty$ ma il modo formale di risolvere questo tipo di forme indeterminate e' quello del **raccoglimento del termine di grado maggiore**.  

```math
\displaystyle{\lim_{x\to -\infty}} (4x^2-2x+3) = 4x^2\bigg(1 -\cancel{\dfrac{1}{2x}}+\cancel{\dfrac{3}{4x^2}}\bigg) = +\infty
```

I termini con l'incognita al denominatore tendono a zero restando il termine con il grado maggiore $4x^2$ che tende invece a $+\infty$  
