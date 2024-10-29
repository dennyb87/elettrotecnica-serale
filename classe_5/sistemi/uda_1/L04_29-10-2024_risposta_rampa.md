# Risposta alla rampa  

![ramp_fun_10](https://github.com/user-attachments/assets/b98d6902-8d7d-4fb9-9f8a-a6309d43f944)  

Si vuole esaminare la risposta di un sistema con $G(s) = \dfrac{2}{s+5}$ ad una rampa di pendenza $10t \cdot u(t)$  

$V_{in}(t) = 10t \cdot u(t) \implies V_{in}(s) = \dfrac{10}{s^2}$  


$V_{out}(s) = G(s)\cdot V_{in}(s) = \dfrac{2}{s+5} \cdot \dfrac{10}{s^2} = \dfrac{20}{s^2(s+5)}$  


### Scomposizione in frazioni parziali  

Quando il prodotto di polinomi al denominatore e' di grado maggiore di 1, oppure se espandendolo in un polinomio $s^2(s+5) = s^3+5s$ e' di grado maggiore di 2, allora la scomposizione in frazioni parziali dovra' tenere conto di una frazione in piu'. In generale il numero di frazioni necessarie per la corretta scomposizione in frazioni parziali e' uguale al grado del polinomio al denominatore, in questo caso...  

$V_{out}(s) = \dfrac{20}{s^2(s+5)} = \dfrac{A}{s}+\dfrac{B}{s^2}+\dfrac{C}{s+5}$  

$V_{out}(s) = \dfrac{As(s+5)+B(s+5)+Cs^2}{s^2(s+5)} = \dfrac{As^2+5As+Bs+5B+Cs^2}{s^2(s+5)}$  

$V_{out}(s) = \dfrac{s^2(A+C)+s(5A+B)+5B}{s^2(s+5)}$  

Mettiamo a sistema...  

$$
\begin{cases}
  \begin{aligned}
    A+C &= 0 \\
    5A+B &= 0 \\
    5B &= 20 \\
  \end{aligned}
\end{cases}
$$

$$
\begin{cases}
  \begin{aligned}
    C &= \dfrac{4}{5} \\
    A &= -\dfrac{4}{5} \\
    B &= 4 \\
  \end{aligned}
\end{cases}
$$


$V_{out}(s) = -\dfrac{0.8}{s} + \dfrac{4}{s^2}+\dfrac{0.8}{s+5}$  

$V_{out}(t) = \underbrace{-0.8u(t)+4t \cdot u(t)}_{termine\ a\ regime} \underbrace{+0.8e^{-5t}u(t)}_{termine\ transitorio}$  

![ramp_fun_10_response](https://github.com/user-attachments/assets/7e742799-b05a-4bd7-8a84-9457f752976d)  

In generale si nota che nella risposta c'e' l'impronta del segnale in ingresso. Si ha un piccolo transitorio di durata...  

$5\tau = 5\frac{1}{a} = 5\frac{1}{5} = 1\ s$  

dopo il quale il sistema si considera a regime in quanto il termine transitorio $+0.8e^{-5t}u(t)$ e' pressoche' zero.  

