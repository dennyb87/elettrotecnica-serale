# Derivata di una costante  

La derivata di una costante e' zero in quanto il rapporto incrementale non puo' che essere sempre zero, cosi' come e' zero la pendenza della retta tangente, per cui se $f(x) = c$ allora...  

$f^\prime(x) = 0$  

Mentre se la funzione contiene una costante e' dimostrabile che questa costante puo' essere estratta per semplicita' dall'operatore di derivazione. Quindi data $f(x) = c\cdot g(x)$ allora...  

$f^\prime(x) = c\cdot g^\prime(x)$  

Si dimostra notando che la costante $c$ non dipende da $h$ percio' e' possibile portarla fuori dal limite.  

$$
\begin{aligned}
    f^\prime(x) &= \displaystyle{\lim_{h \to 0}\ \dfrac{c\cdot g(x+h)-c\cdot g(x)}{h}}\\
    \\
    &= \displaystyle{\lim_{h \to 0}\ c\cdot\dfrac{g(x+h)-g(x)}{h}}\\
    \\
    &= c\cdot\displaystyle{\lim_{h \to 0}\ \dfrac{g(x+h)-g(x)}{h}}\\
    \\
    &= c\cdot g^\prime(x)
\end{aligned}
$$


## Cenni derivate e limiti notevoli  

Consideriamo $f(x) = \sin(2x)$ e calcoliamo la derivata con $x_0 = 0$  

$$
\begin{aligned}
    f^\prime(x) &= \displaystyle{\lim_{h \to 0}\ \dfrac{f(x+h)-f(x)}{h}}\\
    \\
    &= \displaystyle{\lim_{h \to 0}\ \dfrac{\sin\bigg[2\cdot(0+h)\bigg]-\sin(2\cdot 0)}{h}}\\
    \\
    &= \displaystyle{\lim_{h \to 0}\ \dfrac{\sin(2h)-0}{h}}\\
    \\
    &= \displaystyle{\lim_{h \to 0}\ \dfrac{\sin(2h)}{h}}\\
\end{aligned}
$$

In apparenza sembrerebbe una forma indeterminata $\dfrac{0}{0}$ ma dato che $h \to 0$ possiamo applicare l'approssimazione per angoli piccoli dove $\sin \theta \simeq \theta$. Moltiplichiamo quindi per $\frac{2}{2}$ facendo diventare il denominatore uguale all'angolo che come abbiamo detto tende a zero ed e' quindi molto piccolo, percio...  

$f^\prime(x) = \displaystyle{\lim_{h \to 0}\ \dfrac{\sin(2h)}{h}}\cdot \dfrac{2}{2} = \dfrac{\sin(2h)}{2h} \cdot 2 = \cancel{\dfrac{2h}{2h}}\cdot 2 = 2$  
