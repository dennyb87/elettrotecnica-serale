# Dominio di funzioni trigonometriche  

![arcsin_vs_sin](https://github.com/user-attachments/assets/1e0baf9a-72d0-44ee-9c18-3748d203bad9)

La funzione $\sin(x)$ accetta un qualsiasi angono in ingresso percio' il dominio e' tutto $\mathbb{R}$. Il codominio invece sappiamo essere $[-1,\ 1]$ e vediamo infatti la funzione oscillare sull'asse delle ascisse.  

La sua funzione inversa e' l'arcoseno o $\arcsin(x)$ dove invertendo dominio con codominio, accettera' in ingresso $[-1,\ 1]$. Il codominio invece, non essendo una fuzione biettiva non sara' piu' $\mathbb{R}$ in quanto esistono un infinito numero di angoli che hanno lo stesso $sin(x)$. Percio' il codominio di $\arcsin(x)$ resta necessariamente confinato in $\bigg[-\dfrac{\pi}{2},\ \dfrac{\pi}{2} \bigg]$  


$y = \arcsin(e^x-1)$  

Conoscendo il dominio dobbiamo allora porre $-1 \le e^x-1 \le 1$ per cui mettendo a sistema...  

$$
\begin{cases}
  \begin{aligned}
    e^x-1 &\ge -1 \\
    e^x-1 &\le 1 \\
  \end{aligned}
\end{cases}
$$

$$
\begin{cases}
  \begin{aligned}
    e^x &\ge 0 \\
    e^x &\le 2 \\
  \end{aligned}
\end{cases}
$$

La prima e' sempre soddisfatta in quanto l'esponenziale ha un asistoto sull'asse delle ascisse per cui e' sempre maggiore di zero. Mentre alla seconda si applica un logaritmo naturale a entrambe i membri...  

$\ln e^x \le \ln 2 \implies x \le \ln 2$  

Si ha allora che il dominio e':  

$D: x \in (-\infty,\ \ln 2]$  
