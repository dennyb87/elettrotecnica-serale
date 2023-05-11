# Sistemi di equazioni  

Abbiamo notato che per trovare la soluzione di un sistema di equazioni a due incognite ci servono almeno due equazioni. Questo si puo' intuire se ci rendiamo conto che un'equazione a due incognite rappresenta una retta.  

$x + 3y = 6$  

Se abbiamo due rette diverse, con pendenza diversa, e' allora possibile trovare le incognite che individuano il loro punto di intersezione, ovvero la soluzione del sistema.    

$$
\begin{cases}
  \begin{aligned}
    x + 3y &= 6 \\
    2x + 2y &= 4
  \end{aligned}
\end{cases}
$$

![2eq_system](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/5d1e7084-6e0b-4d44-aba2-786e31755b92)  

Nel momento in cui il numero di incognite passa da due a tre, allora l'equazione individua un piano in uno spazio tridimensionale $(x, y, z)$.  

$4x + 5y + 6z = 20$  

![3d_plane](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ce82f6d6-cebb-4bcb-99b3-4eeeadcc318f)  

La soluzione di un sistema di tre equazioni a tre incognite sara' allora quel punto, se esiste, che individua l'intersezione dei tre piani nello spazio tridimensionale.  

$$
\begin{cases}
  \begin{aligned}
    4x + 5y + 6z &= 20 \\
    20x + y + 4z &= 5 \\
    2x + 30y + 2z &= 8
  \end{aligned}
\end{cases}
$$

![3d_planes_intersection](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/39633ff2-07aa-4bae-9ddc-2ccfd597de21)  

## Esempio in due dimensioni  

Consideriamo il seguente problema:  

> L'area di un quadrato e di un rettangolo sono uguali.
> La base del rettangolo supera di 5cm quella del quadrato.
> L'altezza del rettangolo e' la meta' di quella del quadrato.

Riscriviamo il problema nel linguaggio matematico.

>L'area di un quadrato e di un rettangolo sono uguali.  

$\ell^2 = b \cdot h$  

> La base del rettangolo supera di 5cm quella del quadrato.  

$b = 5 + \ell$  

> L'altezza del rettangolo e' la meta' di quella del quadrato.  

$h = \dfrac{1}{2}\ell$  

Abbiamo allora tre equazioni e tre incognite che possiamo mettere a sistema per trovare la soluzione, ovvero i valori delle incognite che soddisfano tutte le equazioni del sistema.  

$$
\begin{cases}
  \begin{aligned}
    \ell^2 &= b \cdot h \\
    b &= 5 + \ell \\
    h &= \dfrac{1}{2}\ell
  \end{aligned}
\end{cases}
$$

Procediamo con il metodo di sostituzione per trovare $\ell$.  

$\ell^2 = b \cdot h$  

$\ell^2 = (5 + \ell) \cdot \dfrac{1}{2}\ell$  

$\ell^2 = \dfrac{\ell(5 + \ell)}{2}$  

$\ell^2 = \dfrac{\ell^2 + 5\ell)}{2}$  

$\cancel{2}\ell^2 = \cancel{\ell^2} + 5\ell$  

$\ell^2 - 5\ell = 0$  

Risolviamo l'equazione di secondo grado trovando che le soluzioni possibili sono $\ell \in \lbrace 0; 5 \rbrace$ ma possiamo escludere zero in quanto avrebbe poco senso come misura del lato di un quadrato, percio' possiamo affermare che $\ell = 5\ cm$.  

Scopriamo allora che...  

$b = 5 + \ell = 5 + 5 = 10\ cm$  

$h = \dfrac{1}{2}\ell = \dfrac{1}{2}5 = 2.5\ cm$  

Se volessimo visualizzare il sistema otterremmo allora un grafico di questo tipo, in cui la prima equazione descrive una parabola con asse di simmetria orizzontale.  

![3var_system](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/5a2d7fbe-740a-42aa-b1cc-c5c15f657936)