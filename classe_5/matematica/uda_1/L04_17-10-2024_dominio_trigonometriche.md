# Dominio di funzioni trigonometriche  

## Seno e arcoseno  

![sinarcsin](https://github.com/user-attachments/assets/a8d75cdc-6f11-4232-868a-55839f1736bd)  

La funzione $\sin(\alpha)$ accetta un qualsiasi angono in ingresso percio' il dominio e' tutto $\mathbb{R}$. Il codominio invece sappiamo essere $[-1,\ 1]$ e vediamo infatti la funzione oscillare sull'asse delle ascisse.  

La sua funzione inversa e' l'arcoseno o $\arcsin(x)$ dove invertendo dominio con codominio, accettera' in ingresso $[-1,\ 1]$. Il codominio invece, non essendo una fuzione biettiva non sara' piu' $\mathbb{R}$ in quanto esistono un infinito numero di angoli che hanno lo stesso $sin(\alpha)$. Percio' il codominio di $\arcsin(x)$ resta necessariamente confinato in $\bigg[-\dfrac{\pi}{2},\ \dfrac{\pi}{2} \bigg]$  


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

## Tangente e arcotangente  

![tanarctan](https://github.com/user-attachments/assets/4969c0f4-0f1c-4840-b43e-5fc00078269e)  

Essendo $\tan(\alpha)$ definito come $\dfrac{\sin(\alpha)}{\cos(\alpha)}$ si hanno asintoti verticali ogni volta che $\cos(\alpha) = 0$ ovvero per ogni $\alpha = \dfrac{\pi}{2}+k\pi$ con $k \in \mathbb{N}$. Il dominio sara' allora...  

$D: \mathbb{R}\ \backslash \ \bigg\lbrace \dfrac{(2k+1)\pi}{2} \ \forall \ k \in \mathbb{Z} \bigg\rbrace$  

Il codominio di $\tan(\alpha)$ e' invece tutto $\mathbb{R}$. E' possibile far approcciare $\alpha$ ad uno degli asintoti verticali senza mai toccarlo per cui non esiste un valore di $y$ per il quale non sia possibile trovare un angolo $\alpha$ tale che $\tan(\alpha) = y$  

Analogamente all'arcoseno, il codominio dell'arcotangente resta confinato in in $\bigg[-\dfrac{\pi}{2},\ \dfrac{\pi}{2} \bigg]$  
