# Calcolo del valore medio di un segnale    

Se si traccia l'andamento di un valore che varia nel tempo si puo' ottenere un  
grafico di questo tipo, con il tempo sull'asse delle $x$ e il valore sull'asse delle $y$

![grafici_e_segnali_fig1](https://user-images.githubusercontent.com/7195133/206120351-35cf074b-2ab9-4ae4-a6b6-d2b57f9c0d68.jpg)


Si nota immediatamente che l'area sotto la curva puo' essere vista come un insieme  
di rettangoli e triangoli, oppure rettangoli e trapezi.  
In entrambe i casi si puo' calcolare l'area totale sotto la curva semplicemente  
sommando appunto le aree dei poligoni sotto la curva stessa, nel nostro caso  
rettangoli $A_{r1}, A_{r2}$ e dei trapezi $A_{t1}, A_{t2}$  

Ricordiamo la formula per il calcolo dell'area di un rettangolo $A_r = a \cdot b$  
e la formula per l'area di un trapezio $A_t = \frac{(a + b) \cdot h}{2}$  

$A_{r1} = 4 \cdot 8 = 32$  
$A_{r2} = 4 \cdot 12 = 48$  
$A_{t1} = \frac{(4 + 12) \cdot 4}{2} = 32$  
$A_{t2} = \frac{(2 + 12) \cdot 8}{2} = 56$  

Troviamo quindi l'area totale:  

$A = A_{r1} + A_{r2} + A_{t1} + A_{t2} = 32 + 48 + 32 + 56 = 168$  

Adesso per trovare il valore medio non ci resta che dividere l'area per il tempo di osservazione.  

$V_{medio} = \frac{Area}{T_{oss}} = \frac{A}{\Delta t} = \frac{168}{24} = 7$  

In questo grafico si ha quindi un valore medio di $7$.

# Esempio con valore negativo  

![grafici_e_segnali_fig2](https://user-images.githubusercontent.com/7195133/206120274-db05361c-e7a0-4603-a808-a647aba0b4f6.jpg)

In caso di valori negativi e quindi area negativa il procedimento resta invariato.  
Si fa la somma algebrica delle aree ricordandoci che quelle negative vanno sottratte.  

$A^+ = \frac{10 \cdot 10}{2} = 50$  
$A^- = \frac{5 \cdot 20}{2} = 50$  

$V_{medio} = \frac{Area}{T_{oss}} = \frac{A^+ - A^-}{\Delta t} = \frac{50 - 50}{20} = \frac{0}{20} = 0$  

Il valore medio in questo caso e' quindi zero.

# Calcolo velocita' di variazione  

La velocita' di variazione ci dice quanto una grandezza aumenta o diminuisce in  
un intervallo di tempo e.g. dire che si viaggia ad una velocita' di $10\ m/s$ equivale  
a dire che per ogni secondo vengono percorsi $10$ metri, ovvero i metri percorsi  
aumentano di 10 per ogni secondo che passa.  


L'andamento di una macchina che parte a $1\ m/s$ e che dopo $10s$ si arresta per $5s$  
e poi torna al punto di partenza ad una velocita' maggiore puo' essere rappresententata  
come segue.  

![grafici_e_segnali_fig3](https://user-images.githubusercontent.com/7195133/206268198-8f557520-bae8-4350-a708-5db106a63b20.jpg)  

Sull'asse delle $x$ abbiamo il tempo $t$ mentre sull'asse delle $y$ abbiamo i metri $m$.  
Il rapporto tra i metri percorsi e i secondi passati $v = \frac{\Delta y}{\Delta x}$ ci dice appunto la  
velocita' con cui la macchina si sta' muovendo.  
Si nota immediatamente che la macchina si muove con $3$ diverse velocita'.  
Per calcolarle non bisogna fare altro che calcolare i metri percorsi nell'intervallo  
di tempo, e dividerli per l'intervallo di tempo considerato.  

Per esempio nei primi $10$ secondi vediamo che la macchina ha percorso $10$ metri.  
Si arriva a questa conclusione semplicemente calcolando la differenza tra i metri  
percorsi al secondo $10$, ovvero in posizione finale $y_f$, e i metri percorsi al  
secondo $0$, ovvero in posizione iniziale $y_i$.  
Si fa lo stesso per trovare il tempo di osservazione $t_f - t_i$

$v_1 = \frac{y_f - y_i}{t_f - t_i} = \frac{10 - 0}{10 - 0} = \frac{10}{10} = 1\ m/s$  
$v_2 = \frac{y_f - y_i}{t_f - t_i} = \frac{10 - 10}{15 - 10} = \frac{0}{5} = 0\ m/s$  
$v_3 = \frac{y_f - y_i}{t_f - t_i} = \frac{0 - 10}{20 - 15} = \frac{-10}{5} = -2\ m/s$  

La macchina si muove ad $1\ m/s$ per $10s$ poi resta ferma per $5s$ quindi $0\ m/s$,  
infine  riparte tornando in posizione di partenza ad una velocita' di $2\ m/s$.  
Il segno negativo ci indica la direzione: se positivo ci stiamo allontanando dal  
punto di partenza, se negativo vi stiamo invece tornado.  
