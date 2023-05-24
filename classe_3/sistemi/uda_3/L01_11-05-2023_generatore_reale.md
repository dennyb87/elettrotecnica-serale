# Modello di un generatore reale  

![generatore_reale](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/46f20803-c75e-457e-8169-07f129dc43d2)  

Al contrario di un generatore ideale, il **generatore reale** viene modellato come un generatore $V_s$ in serie ad una resistenza interna $R_s$. Derivando la tensione ai capi del generatore reale $V_{out}$ grazie alla seconda legge di Kirchhoff si nota immediatamente che l'equazione descrive una retta con pendenza negativa.  

$V_{out} = -R_s \cdot I + V_s$  

![generatore_reale_grafico](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/8d1cb6b6-ca0d-414d-ae56-caf3c65e6d1b)  

Tracciando il grafico diventa ovvio che la tensione $V_{out}$ a vuoto e' sempre uguale a $V_s$ in quanto con corrente zero non si ha nessuna caduta di potenziale su $R_s$.  

In presenza di corrente invece si ha invece una caduta di tensione su $R_s$ che aumenta all'aumentare della corrente. Quando la corrente e' tale da rendere la tensione ai capi del generatore $V_{out} = 0$ siamo allora di fronte ad un cortocircuito, dove la corrente e' massima e la tensione ai capi del generatore e' zero.  

| Stati di fuzionamento |           |                 |
| --------------------- | --------- | --------------- |
| A vuoto               | $I = 0$   | $V_{out} = V_s$ |
| A carico              | $I > 0$   | $V_{out} < V_s$ |
| In cortocircuito      | $I_{max}$ | $V_{out} = 0$   |
