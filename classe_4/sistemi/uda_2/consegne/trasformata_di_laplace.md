# Trasformata e antitrasformata di Laplace  

### ES 1 - Determinare la trasformata di Laplace delle seguenti funzioni f(t) scrivendo F(s) come rapporto di polinomi in s  

$f_a(t) = 10 \cdot u(t)-e^{0.2t}u(t)$  
$f_b(t) = 10t \cdot u(t)+e^{0.2t}u(t)$  
$f_c(t) = 10e^{20t}u(t)-4e^{-5t}u(t)$  

$F_a(s) = \dfrac{10}{s}-\dfrac{1}{s-0.2} = \dfrac{10(s-0.2)-s}{s(s-0.2)} = \dfrac{9s - 2}{s^2-0.2s}$  

$F_b(s) = \dfrac{10}{s^2}+\dfrac{1}{s+0.2} = \dfrac{10(s+0.2)+s^2}{s^2(s+0.2)} = \dfrac{s^2+10s+2}{s^3+0.2s^2}$  

$F_c(t) = \dfrac{10}{s-20}-\dfrac{4}{s+5} = \dfrac{10(s+5) -4(s-20)}{(s-20)(s+5)} = \dfrac{10s+50-4s+80}{s^2+5s-20s-100} = \dfrac{6s+130}{s^2-15s-100}$  

### ES 2 - Antitrasformare le seguenti funzioni  

$F_a(s) = \dfrac{5s+20}{s(s+2)} = \dfrac{A}{s} + \dfrac{B}{s+2}$  

$f_a(t) =$  
