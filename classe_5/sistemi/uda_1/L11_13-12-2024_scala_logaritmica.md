# Scala logaritmica  

![linea_scale](https://github.com/user-attachments/assets/33b4490a-53cd-4714-b258-ddf31a0a3bba)

La scala logaritmica viene utilizzata per rappresentare sullo stesso grafico grandezze molto piccole e grandezze molto grandi. Nel caso in figura si ha una serie di questo tipo...  

| $x$ | $y$  |
| --- | ---- |
| 1   | 120  |
| 2   | 4    |
| 3   | 1500 |
| 4   | 37   |

...in cui diventa difficile rappresentare sullo stesso grafico grandezze che spaziano intervalli di valori molto grandi. Per ovviare a questo problema si cambia la scala dell'asse delle ordinate riportando i valori equidistanti di **logaritmi in base 10**. Infine invece di tracciare sul grafico i valori reali di $y$ si tracciano i valori di $\log y$  

![logarithmic_scale](https://github.com/user-attachments/assets/fda68088-43ee-43aa-8fc1-f3bc4138af7d)  

Si ha allora che le coordinate diventano quindi...  

| $x$ | $\log y$ | $y$                |
| --- | -------- | ------------------ |
| 1   | 2.08     | $10^{2.08} = 120$  |
| 2   | 0.6      | $10^{0.6} = 4$     |
| 3   | 3.18     | $10^{3.18} = 1500$ |
| 4   | 1.57     | $10^{1.57} = 37$   |


E' importante notare come la scala logaritmica permetta di ottenere una scala lineare per valori che altrimenti  crescono in modo esponenziale.  

|                   |                           |
| ----------------- | ------------------------- |
| $\log  100 = 2$   | $\implies 10^2 = 100$     |
| $\log  10 = 1$    | $\implies 10^1 = 10$      |
| $\log  1 = 0$     | $\implies 10^0 = 1$       |
| $\log  0.1 = -1$  | $\implies 10^{-1} = 0.1$  |
| $\log  0.01 = -2$ | $\implies 10^{-2} = 0.01$ |