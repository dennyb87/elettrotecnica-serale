# Mappe di Karnaugh  

Data una funzione booleana, o la relativa tabella di verita', e' possibile rappresentarla graficamente in maniera compatta attraverso quella che viene chiamata mappa di Karnaugh.  

Per costruire la mappa basta disegnare $2^n$ dove $n$ e' il numero di variabili in ingresso. Ad ogni casella viene assegnata una coordinata che coincide con le disposizioni con ripetizioni delle variabili in ingresso.  

| c\ab  | 00  | 01  | 11  | 10  |
| ----- | --- | --- | --- | --- |
| **0** |     | $1$ | $1$ |     |
| **1** |     | $1$ | $1$ | $1$ |

E' importante ordinare le coordinate delle caselle in modo che differiscano tra di esse di una sola variabile. Questo ci permette di effettuare raggruppamenti e.g. 2,4,8 caselle etc... trovando infine la forma minima della funzione.  

| c\ab  | 00  | 01               | 11               | 10  |
| ----- | --- | ---------------- | ---------------- | --- |
| **0** |     | $\color{red}{1}$ | $\color{red}{1}$ |     |
| **1** |     | $1$              | $1$              | $1$ |

Non e' per niente banale, ma effettuando un primo raggruppamento diventa evidente che la risultante somma di mintermini e' un'espressione in cui la variabile non costante produce l'elemento neutro del prodotto logico, ovvero $1$ per cui puo' essere ignorata:  

$\overline{A}B\overline{C} + AB\overline{C} = B\overline{C} \cdot (A+ \overline{A}) = B\overline{C}$  

Possiamo allora dedurre che i raggruppamenti possono essere fatti direttamente per via grafica, scrivendo solo quei termini che restano costanti tra le caseselle raggruppate, in questo caso $B\overline{C}$.  

| c\ab  | 00  | 01               | 11               | 10  |
| ----- | --- | ---------------- | ---------------- | --- |
| **0** |     | $1$              | $1$              |     |
| **1** |     | $\color{red}{1}$ | $\color{red}{1}$ | $1$ |

Il prossimo raggruppamento mette invece in evidenza:  

$\overline{A}BC + ABC = BC \cdot (\overline{A}+A) = BC$  

| c\ab  | 00  | 01               | 11               | 10  |
| ----- | --- | ---------------- | ---------------- | --- |
| **0** |     | $\color{red}{1}$ | $\color{red}{1}$ |     |
| **1** |     | $\color{red}{1}$ | $\color{red}{1}$ | $1$ |

Possiamo allora fare un raggruppamento da 4 caselle ottenendo:  

$B\overline{C} + BC = B \cdot (\overline{C}+C) = B$  

| c\ab  | 00  | 01  | 11               | 10               |
| ----- | --- | --- | ---------------- | ---------------- |
| **0** |     | $1$ | $1$              |                  |
| **1** |     | $1$ | $\color{red}{1}$ | $\color{red}{1}$ |

Effetuiamo quindi l'ultimo raggruppamento possibile:  

$ABC + A\overline{B}C =AC \cdot (B + \overline{B}) = AC$  

Scopriamo allora che la **forma minima** di questa funzione e':  

$Y = B + AC$  
