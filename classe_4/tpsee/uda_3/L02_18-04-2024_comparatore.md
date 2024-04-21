# Comparatore  

![comparator](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/40e8fa6b-4bd8-455d-a897-d580a7603a4e)  

Il comparatore e' un dispositivo con due ingressi ed una uscita in grado di confrontare due segnali in ingresso fornendo in uscita un livello logico che rappresenta il risultato del confronto.  

![comparator_schema](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f41def16-23cb-44b9-a409-8827a5305e12)  

Il simbolo **ground** (*massa*) rappresenta il **riferimento a potenziale zero**, ovvero una linea comune di riferimento per la misura delle tensioni.  

La differenza tra l'ingresso e il riferimento prende il nome di $V_d$  

$V_d = V_{IN} - V_{REF}$  

Il funzionamento del comparatore e' allora definito come segue:  

$$
V_{out} =
\begin{cases}
  \begin{aligned}
    V_{cc}\ \ &V_d \gt 0\\
    0\ \ &V_d \le 0
  \end{aligned}
\end{cases}
$$

| $V_{IN}$ | $V_{REF}$ | $V_d$ | $V_{out}$ |
| -------- | --------- | ----- | --------- |
| 2        | 1         | 1     | 10        |
| 5        | 2         | 3     | 10        |
| 2        | 5         | -3    | 0         |
| 3        | 3         | 0     | 0         |

![comparator_function](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9f6cbc88-6561-4e09-b1ad-a05669249ac5)  

Data la natura della loro funzione questi dispositivi vengono anche detti amplificatori operatorazionali.  
