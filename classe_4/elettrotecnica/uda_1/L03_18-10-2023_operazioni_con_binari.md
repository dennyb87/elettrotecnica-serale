# Somma binaria  

La somma binaria si svolge in modo analogo a quella nel sistema decimale, con la differenza che essendo 1 la cifra piu' alta si ha un riporto ogni volta che la somma supera tale valore.  

$$
\begin{aligned}
    ^1\ 1\ \\
      +\ 1\ \\
    \hline
    1\ 0\ \\
\end{aligned}
$$

# Prodotto binario  

Questa operazione segue le stesse regole di quella decimale.  

$$
\begin{aligned}
    1\ 0\ 1\ \\
\times\ 1\ 0\ \\
    \hline
      0\ 0\ 0\ \\
    +\ 1\ 0\ 1\ \ \ \ \\
    \hline
      1\ 0\ 1\ 0\ \\
\end{aligned}
$$

# Intro algebra di Boole  

I circuiti logici digitali sono essenzialmente dispositivi in grado di assumere due soli stati, questi stati dipendono da una grandezza fisica, spesso la tensione. A questa vengono associati due valori, o intervalli di funzionamento:  

* livello logico alto $\implies$ 1
* livello logico basso $\implies$ 0

Infine per non lasciare spazio ad ambiguita' esiste un intervallo dove lo stato non e' determinabile.  

![livelli_logici](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/e0ecda68-3fee-4aaa-83dd-3df90c1e15c4)  

Per questo motivo anche se la somma binaria prevede $1 + 1 = 0$ con riporto di uno, al livello logico si ha che $1 + 1 = 1$  

## Porta logica OR (somma logica)  

![somma_logica_or](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7078c519-e6b6-411e-b068-ae319c5360a6)  
![or_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/d5a9e7eb-c55a-41c4-ae8c-e662da57e786)  

| A   | B   | Y   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 1   |
| 1   | 0   | 1   |
| 1   | 1   | 1   |

## Porta logica AND (prodotto logico)  

![prodotto_logico_and](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b8465d23-f11d-4b04-b216-379d58a1c9af)  
![and_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7b9c4651-af4f-4591-8b32-5be1f0480a87)  

| A   | B   | Y   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 1   |
