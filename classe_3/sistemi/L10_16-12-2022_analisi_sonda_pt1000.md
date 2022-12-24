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


## Calcolo della temperatura a resistenza zero  

Data la curva caratteristica della sonda si puo' intuire che deve esistere una  
temperatura a cui la retta interseca l'asse delle ascisse e la resistenza diventa  
quindi zero.  

![sonda_pt_1000_curva_caratteristica](https://user-images.githubusercontent.com/7195133/196776916-a970bb43-232b-44f1-a02b-8b3ab2f3d15d.jpg)

Conoscendo la formula per il calcolo della resistenza, possiamo allora porre $R_T = 0$  
e riarrangiare l'equazione per trovare $T$ ovvero la temperatura a cui la resistenza e' zero.   

$R_T = R_0 \cdot (1 + \alpha \cdot T)$  

$0 = R_0 \cdot (1 + \alpha \cdot T)$  

$0 = R_0 + R_0 \cdot \alpha \cdot T$  

$- R_0 = R_0 \cdot \alpha \cdot T$  

$- \dfrac{R_0}{R_0 \cdot \alpha} = T$  

$- \dfrac{1}{\alpha} = T$  


Si intuisce immediatamente allora che la temperatura a cui la resistenza diventa zero  
non e' altro che il reciproco di $\alpha$ per $-1$ ovvero:  

$T = - \dfrac{1}{\alpha} = -1 \cdot \dfrac{1}{3.9083 \cdot 10^{-3}} \simeq -255.87\ ^\circ C$  

Infatti se sostiuiamo $-255.87\ ^\circ C$ nell'equazione per trovare la resistenza si ottiene zero.    

$R_T = R_0 \cdot (1 + \alpha \cdot T) = 1000 \cdot (1 + 3.9083 \cdot 10^{-3} \cdot -255.87) = 1000 \cdot (1 - 1) \simeq 0\ \Omega$ 