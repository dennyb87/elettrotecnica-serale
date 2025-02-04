# Studio della discontinuita' di una funzione  

![fun_continuita](https://github.com/user-attachments/assets/2d990d74-eabd-4afb-a518-9cbf3022d331)  

$$
f(x) =
\begin{cases}
  \begin{aligned}
    \dfrac{1}{x-1} &\ \ \ ]-\infty,1[\\
    \log_2(x-1) &\ \ \ ]1,3[\\
    2x-5 &\ \ \ ]3,7[\\
    8 &\ \ \ ]7,+\infty[\\
  \end{aligned}
\end{cases}
$$

Data la funzione $f(x)$ se ne vuole studiare i punti di discontinuita'. Agli estremi $\pm\infty$ e' continua percio' procediamo ad esaminare cosa succede ai confini degli intervalli interni. Notando che la funzione non e' definita $\forall\ x \in \{1, 3, 7\}$ deduciamo che la funzione ha 3 *"buchi"*. Valutiamo quindi i rispettivi limiti da destra e da sinistra dei valori ai confini degli intervalli interni...  

$\displaystyle{\lim_{x\to 1^-}}\ \dfrac{1}{x-1} = \dfrac{1}{1^--1} = \dfrac{1}{0^-} =-\infty$  

$\displaystyle{\lim_{x\to 1^+}}\ \log_2(x-1) = \log_2(1^+-1) = \log_2(0^+) = -\infty$  

Con $x = 1$ si ha allora una discontinuita' di **seconda specie** in quanto almeno uno dei due limiti e' infinito.  

$\displaystyle{\lim_{x\to 3^-}}\ \log_2(x-1)= \log_2(3^--1)=\log_2(2)=1$  

$\displaystyle{\lim_{x\to 3^+}}\ 2x-5 =2\cdot3 -5 =1$  

Il limite esiste ma non coincide con $f(3)$ che invece non esiste, percio' siamo di fronte ad una discontinuita' di **terza specie**.  

$\displaystyle{\lim_{x\to 7^-}}\ 2x-5 =2\cdot7 -5 =9$  

$\displaystyle{\lim_{x\to 7^+}}\ 8 = 8$  

Qui abbiamo un salto percio' si tratta di una discontinuita' di **prima specie**.  
