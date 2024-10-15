# Risposta ai segnali canonici  

Conoscendo la funzione di trasferimento di un sistema nel dominio di Laplace $G(s) = \dfrac{2}{s+5}$ si vuole esaminare la risposta ai segnali canonici: impulso, gradino e rampa, considerando i segnali di ampiezza $10$.  

### Risposta all'impulso unitario  

$x(t) = 10 \cdot \delta(t) \implies X(s) = 10$  

$Y(s) = X(s) \cdot G(s) = 10 \cdot \dfrac{2}{s+5} = 20 \cdot \dfrac{1}{s+5}$  

$y(t) = 20 \cdot e^{-5t}u(t)$  

![unit_impulse_response](https://github.com/user-attachments/assets/4bf03697-7cea-445c-9263-b482a9868a95)  

### Risposta al gradino unitario  

$x(t) = 10 \cdot u(t) \implies X(s) = \dfrac{10}{s}$  

$Y(s) = X(s) \cdot G(s) = \dfrac{10}{s} \cdot \dfrac{2}{s+5} = \dfrac{20}{s(s+5)}$  

Per tornare nel dominio del tempo e' necessario riscrivere $Y(s)$ in frazioni parziali antitrasformabili.  

$Y(s) = \dfrac{20}{s(s+5)} = \dfrac{A}{s} + \dfrac{B}{s+5}$  

$Y(s) = \dfrac{A(s+5)+Bs}{s(s+5)} = \dfrac{As+5A+Bs}{s(s+5)} = \dfrac{s(A+B)+5A}{s(s+5)}$  

Per rendere vera l'equazione il numeratore deve essere uguale a $20$ per cui mettendo a sistema...  

$$
\begin{cases}
  \begin{aligned}
    A+B &= 0 \\
    5A &= 20 \\
  \end{aligned}
\end{cases}
$$

Si ha allora che...  

$Y(s) = \dfrac{4}{s} - \dfrac{4}{s+5}$  

$y(t) = 4 \cdot u(t) -4 \cdot e^{-5t}u(t)$  

![unit_step_fun_response](https://github.com/user-attachments/assets/4a90da4e-ed84-481e-a1d7-ea3520590cf5)  

