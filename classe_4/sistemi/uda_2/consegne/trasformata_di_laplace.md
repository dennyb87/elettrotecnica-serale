# Trasformata e antitrasformata di Laplace  

### ES 1 - Determinare la trasformata di Laplace delle seguenti funzioni f(t) scrivendo F(s) come rapporto di polinomi in s  

$f_a(t) = 10 \cdot u(t)-e^{0.2t}u(t)$  
$f_b(t) = 10t \cdot u(t)+e^{0.2t}u(t)$  
$f_c(t) = 10e^{20t}u(t)-4e^{-5t}u(t)$  

$F_a(s) = \dfrac{10}{s}-\dfrac{1}{s-0.2} = \dfrac{10(s-0.2)-s}{s(s-0.2)} = \dfrac{9s - 2}{s^2-0.2s}$  

$F_b(s) = \dfrac{10}{s^2}+\dfrac{1}{s+0.2} = \dfrac{10(s+0.2)+s^2}{s^2(s+0.2)} = \dfrac{s^2+10s+2}{s^3+0.2s^2}$  

$F_c(t) = \dfrac{10}{s-20}-\dfrac{4}{s+5} = \dfrac{10(s+5) -4(s-20)}{(s-20)(s+5)} = \dfrac{10s+50-4s+80}{s^2+5s-20s-100} = \dfrac{6s+130}{s^2-15s-100}$  

### ES 2 - Antitrasformare le seguenti funzioni  

$F_a(s) = \dfrac{5s+20}{s(s+2)} = \dfrac{A(s+2)+Bs}{s(s+2)} = \dfrac{As+A2+Bs}{s(s+2)} = \dfrac{(A+B)s+A2}{s(s+2)}$  

$$
(A+B)s + A2 \implies
\begin{cases}
  \begin{aligned}
    A2 &= 20\\
    A+B &= 5
  \end{aligned}
\end{cases}
\implies
\begin{cases}
  \begin{aligned}
    A &= 10\\
    B &= -5
  \end{aligned}
\end{cases}
$$

$F_a(s) = \dfrac{10}{s}-\dfrac{5}{s+2} \implies f_a(t) = 10u(t)-5e^{-2}u(t)$  

***  

$F_b(s) = \dfrac{16}{4s + 40} = \dfrac{A(s+10) + B4}{4(s+10)} = \dfrac{As+10A+B4}{4(s+10)}$  

$$
(A+B)s + A2 \implies
\begin{cases}
  \begin{aligned}
    A &= 0\\
    B &= 4
  \end{aligned}
\end{cases}
$$

$F_b(t) = \dfrac{4}{s+10} \implies f_b(t) = 4e^{-10t}u(t)$  

***  

$F_c(s) = \dfrac{5s+20}{(s-4)(s+2)} = \dfrac{K_1}{s-4} + \dfrac{K_2}{s+2}$  

$P_1 = 4$  
$P_2 = -2$  

$K_1 = \dfrac{5(4)+20}{4 + 2} = \dfrac{40}{6} = \dfrac{20}{3}$  

$K_2 = \dfrac{5(-2)+20}{-2-4} = - \dfrac{10}{6} = -\dfrac{5}{3}$  


$F_c(s) = \dfrac{\frac{20}{3}}{s-4}-\dfrac{\frac{5}{3}}{s+2} \implies f_c(t) = \dfrac{20}{3}e^{4t}u(t)-\dfrac{5}{3}e^{-2t}u(t)$  

### ES 3 - Transitorio di carica e di scarica di un condensatore  

![fad_transitorio_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/aa41fc7a-fe40-4404-9174-f50d09bc723f)  

Si consideri il circuito mostrato in figura dove:  

$E = 20\ V$  
$R = 2\ k\Omega$  
$C = 5\ mF$  

Il deviatore è azionato in modo tale che:  

$$
e(t) = \begin{cases}
  \begin{aligned}
    0;\ t &< 0  \\
    E;\ 0 &\le t \le 60\ s\\
    0;\ t &> 60\ s
  \end{aligned}
\end{cases}
$$

Si chiede di:  

1. disegnare il grafico dell'eccitazione $e(t)$ del circuito RC
2. calcolare la costante di tempo del circuito
3. disegnare l'andamento al variare del tempo della tensione ai capi del condensatore e della
corrente in risposta alla eccitazione $e(t)$

Possiamo tracciare $V_c(t)$ conoscendo la legge di carica del condensatore:  

$V_c(t) = V_f+(V_i-V_f)e^{-\frac{t}{\tau}} \cdot u(t)$  

Si vuole quindi trovare $\tau$ e la durata del transitorio...  

$\tau = RC = 2000 \cdot 0.005 = 10\ s$  
$T_d = 5\tau = 5 \cdot 10 = 50\ s$  

Con Kirchhoff possiamo derivare l'equazione per $i(t)$ che in ogni caso segue la stessa legge della tensione.  

$e(t) = Ri(t) + V_c(t) \implies i(t) = \dfrac{e(t) - V_c(t)}{R}$  

Ma all'istante $t = 0\ s$ la tensione sul condensatore e' zero per cui...  

$i(0) = I_{max} = \dfrac{e(0) - V_s(0)}{R} = \dfrac{e(0) - 0}{R} = \dfrac{20}{2000} = 0.01\ A = 10\ mA$  

![fad_vct_et_transitorio_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/808464f0-bf72-43d4-aa7f-774d3b118528)

![fad_ic_transitorio_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/99fdf53c-d45b-4f5c-8357-c78f05ec8b19)
