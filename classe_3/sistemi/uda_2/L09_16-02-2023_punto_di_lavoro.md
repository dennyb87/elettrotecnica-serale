# Determinazione del punto di lavoro  

Dato un dispositivo ed un carico, il punto di lavoro rappresenta l'intersezione tra la curva tensione-corrente del dispositivo e la retta di carico. Trovare il punto di lavoro ottimale significa allora trovare quel carico che permette di sfruttare il dispositivo al massimo della sua potenza.

Nel caso per esempio di un modulo fotovoltaico e' possibile identificare tre possibili stati di funzionamento:  

* funzionamento a carico
* funzionamento a vuoto
* funzionamento in cortocircuito

## Dati di targa  

Consideriamo i seguenti dati di targa di un **modulo VGS VE172PV**.  

| Descrizione                | Simbolo  | Valore        |
| -------------------------- | -------- | ------------- |
| Irraggiamento incidente    | $G$      | $1000\ W/m^2$ |
| Superficie del dispositivo | $A$      | $2\ m^2$      |
| Potenza di picco           | $P_p$    | $280\ W$      |
| Rendimento                 | $\eta$   | $14.14$ %     |
| Corrente di corto circuito | $I_{sc}$ | $8.2\ A$      |
| Corrente massima STC       | $I_m$    | $7.64\ A$     |
| Tensione a circuit aperto  | $V_{oc}$ | $45.35\ V$    |
| Tensione massima STC       | $V_m$    | $36.85\ V$    |

I dati di targa del dispositivo ci forniscono anche il grafico della tensione-corrente, quindi la curva che descrive la risposta in base al carico. Dal grafico possiamo quindi osservare le grandezze elettriche in gioco in ognuno degli **stati di funzionamento**.  

![curva-tensione-corrente](https://user-images.githubusercontent.com/7195133/219871474-12b1578d-43a7-4f37-9dff-114aa1745132.jpg)  

Si noti che in caso di corto circuito si ha una corrente $I_{sc}$ con tensione zero, mentre in caso di funzionamento a vuoto si ha una grande tensione $V_{oc}$ ma nessuna corrente. Il punto di massima potenza, in inglese *maximum power point* (**MPP**), e' il punto di lavoro ottimale, che permette di sfruttare il dispositivo alla sua potenza massima.  

Sappiamo grazie alla legge di Ohm che a parita' di resistenza, la corrente aumentera' all'aumentare della tensione in modo lineare. Tracciando il grafico di tensione-corrente si presentera' allora una **retta di carico**.  

![ohm_law](https://user-images.githubusercontent.com/7195133/219904387-317a6e3f-da84-48d4-b125-3e0700df354b.jpg)  

Si nota immediatamente che $\dfrac{1}{R}$ e' la pendenza della retta. Allora va da se che per trovare il carico ideale per questo dispositivo ci serve una carico che presenti una resistenza tale che la retta di carico si intersechi con la curva tensione-corrente al punto **MPP** quindi nel nostro esempio:    

$R_m = \dfrac{V_m}{I_m} = \dfrac{36.85}{7.64} \simeq 4.82\ \Omega$  

$P_m = V_m \cdot I_m = R_m \cdot I_m^2 = 4.82 \cdot 7.64^2 \simeq 281.34\ W$  

Un carico da $4.82\ \Omega$ ci permette allora di raggiungere approssimativamente la potenza di picco descritta nei dati di targa $280\ W$.  