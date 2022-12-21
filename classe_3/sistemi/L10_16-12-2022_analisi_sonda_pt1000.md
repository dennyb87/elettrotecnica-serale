# Analisi sonda PT1000  

Vogliamo analizzare il comportamento nel tempo della tensione ai capi della sonda $R_T$
inserita nel circuito in figura.  

![pt1000_analysis](https://user-images.githubusercontent.com/7195133/209002258-d3ef6fed-37df-4496-9501-36d8cddda3b0.jpg)  

Sappiamo che la sonda PT1000 a $0\ ^\circ C$ presenta una resistenza di $1000\Omega$ che variera'  
al variare della temperatura, mentre $R_0$ e' invece una resistenza fissa equivalente.  
Questa configurazione ci permette di intuire velocemente che a $0\ ^\circ C$ la tensione,  
distribuendosi in modo proporzionale alle resistenze in gioco, si dividera' esattamente a meta'.  
Allora cadranno quindi $6V$ su $R_0$ e altrettanti su $R_T$  

Ricordiamo ora la formula per il calcolo della resistenza per la sonda PT1000.  
$R_0$ non e' stata scelta a caso visto che e' uguale a $R_T$ a $0\ ^\circ C$ ed utilizzata quindi  
nella formula.

$\alpha = 3.9083 \cdot 10^{-3}\ ^\circ C^{-1}$  
$R_T = R_0 \cdot (1 + \alpha \cdot T)$  

Andiamo allora a calcolare la tensione su $R_T$ al variare della temperatura.  

![pt1000_voltage_analysis](https://user-images.githubusercontent.com/7195133/209012852-bb43e0db-b781-4cbe-be7f-c10299fe20e0.jpg)  

| $T\ [^\circ C]$ | $R_T\ [V]$ | $V_T\ [V]$ | $V_0\ [V]$ | $V_{tot}\ [V]$ |
| --------------- | ---------- | ---------- | ---------- | -------------- |
| $0$             | $1000.00$  | $6.00$     | $6.00$     | $12$           |
| $10$            | $1039.08$  | $6.12$     | $5.88$     | $12$           |
| $20$            | $1078.17$  | $6.23$     | $5.77$     | $12$           |
| $30$            | $1117.25$  | $6.33$     | $5.67$     | $12$           |
| $...$           | $...$      | $...$      | $...$      | $...$          |


La tabella ci mostra ancora una volta che all'aumentare della temperatura la resistenza  
aumenta, abbiamo gia' visto in passato che aumenta in modo lineare.  

Il grafico invece mette in evidenza che anche la tensione ai capi della sonda varia in modo lineare.  
In particolare mentre la tensione ai capi di $R_T$ aumenta, quella ai capi di $R_0$ diminuisce.  



