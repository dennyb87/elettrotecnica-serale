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
