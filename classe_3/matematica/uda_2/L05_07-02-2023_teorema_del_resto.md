# Teorema del resto  

Il resto della divisione di un polinomio $P(x)$ per un polinomio $x - a$ con $\forall x \in \mathbb{R}$ e' dato dalla valutazione di $P(x)$ con $x = a$ ovvero $P(a)$. Vediamo un esempio per fare chiarezza.  

$P(x): D(x) = (x^3+x^2+x+1):(x+2)$  

$R = P(-2) = (-2)^3+(-2)^2-2+1 = -8+4-2+1 = -5$  

Certamente molto piu' veloce che eseguire la divisione tra polinomi.  
Vediamo ora la dimostrazione di $P(x):(x - a) \implies P(a) = R$.  
La divisione tra polinomi ci dice che:  

$P(x) = Q(x)D(x) + R(x)$  

Ma se $D(x) = (x-a)$ allora $R(x)$ o e' uguale a zero oppure il suo grado e' zero, in ogni caso e' una costante indipendente da $x$ quindi semplicemente $R$ ovvero $P(x) = Q(x)(x-a) + R$.  

$P(a) = Q(a)(a - a) + R = P(a) = Q(a) \cdot 0 + R = R$  

Valutiamo allora $P(x)$ con $x = a$ si nota immediatamente che $P(a) = R$ 



