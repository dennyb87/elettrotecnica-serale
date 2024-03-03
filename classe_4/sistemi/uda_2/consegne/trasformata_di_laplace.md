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

#

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

#

$F_c(s) = \dfrac{5s+20}{(s-4)(s+2)} = \dfrac{K_1}{s-4} + \dfrac{K_2}{s+2}$  

$P_1 = 4$  
$P_2 = -2$  

$K_1 = \dfrac{5(4)+20}{4 + 2} = \dfrac{40}{6} = \dfrac{20}{3}$  

$K_2 = \dfrac{5(-2)+20}{-2-4} = - \dfrac{10}{6} = -\dfrac{5}{3}$  


$F_c(s) = \dfrac{\frac{20}{3}}{s-4}-\dfrac{\frac{5}{3}}{s+2} \implies f_c(t) = \dfrac{20}{3}e^{4t}u(t)-\dfrac{5}{3}e^{-2t}u(t)$  
