# Sulla derivabilita'  

Si vuole far notare che *la derivabilita' implica la continuita* ma non e' necessariamente vero il contrario. Ad esempio la funzione valore assoluto presenta una cuspide, e pur essendo continua, non e' derivabile in $x_0 = 0$  

$$
f(x) = |x| = 
\begin{cases}
    \begin{aligned}
    x\ &\mid x \ge 0\\
    -x &\mid x \lt 0
    \end{aligned}
\end{cases}
$$

![absolute](https://github.com/user-attachments/assets/60fd13ff-aa6a-428b-9c43-8311053b29f1)  


$f^\prime(x) = \displaystyle{\lim_{h\to 0^\pm}}\ \dfrac{f(x_0+h)-f(x_0)}{h} = \dfrac{f(0+h)-f(0)}{h}=\dfrac{|0+h|-|0|}{h}=\dfrac{|h|}{h}$  

Il problema e' che con $x\to 0^-$ si ha che $\dfrac{|h|}{h} = -\dfrac{h}{h} = -1$ mentre con $x\to 0^+$ si ha $\dfrac{|h|}{h} = \dfrac{h}{h} = 1$  

La funzione e' continua ma il limite non esiste percio' non e' derivabile.  

