# Progetto impianto fotovoltaico stand-alone  

Si vuol progettare un impianto fotovoltaico stand-alone da installare sul tetto di una seconda casa off-grid di circa $56\ m^2$ ad uso villeggiatura, ubicata in una zona rurale del comune di Pietrasanta alle coordinate LAT $43.963129$ LONG $10.201176$. Si ipotizza un fabbisogno di energia elettrica giornaliero di $4\ kWh$ che tiene conto di un fattore di sicurezza del 20%. Dato il tipo e l'orientamento del tetto si ipotizza un'inclinazione approssimativa di $30^\circ$ ed un angolo di azimuth di $-45^\circ$ quindi orientato a Sud-Est (Enea utilizza il punto cardinale Sud come riferimento).  

![casa_di_campagna_56m2](https://user-images.githubusercontent.com/7195133/233837334-b19b4d24-239c-408c-8ff1-044e770e394d.jpg)  

![azimuth_approximation](https://user-images.githubusercontent.com/7195133/233838356-4fa0cbcb-190e-4f76-b372-3a99bb5704fa.jpg)  

## Modulo fotovoltaico  

Si vogliono utilizzare moduli **VE172PV-280V** di cui vediamo in tabella le caratteristiche in condizioni standard **STC** ovvero con un irraggiamento di $1000\ W/m^2$, temperatura del modulo di $25^\circ C$, ed un coefficiente di massa d'aria $AM = 1.5$  

|                            |          |            |
| -------------------------- | -------- | ---------- |
| Classe di potenza          | $P_{m}$  | $280\ W$   |
| Efficienza                 | $\eta$   | $14.14$ %  |
| Tensione a circuito aperto | $V_{oc}$ | $45.35\ V$ |
| Corrente di cortocircuito  | $I_{sc}$ | $8.2\ A$   |
| Tensione alla max. potenza | $V_{m}$  | $36.85\ V$ |
| Corrente alla max. potenza | $I_{m}$  | $7.64 A$   |

![pv_curve](https://user-images.githubusercontent.com/7195133/233843035-a12080b1-874f-498c-a8bc-0943049679e6.jpg)


## Calcolo moduli per il fabbisogno energetico   

Utilizziamo gli strumenti di calcolo del sito ENEA per stimare l'irraggiamento giornaliero medio mensile nel luogo di installazione. Assumiamo un coefficiente di riflessione pessimistico uguale a zero, anche se tecnicamente con un inclinazione di $30^\circ$ potremmo beneficiare di una piccola riflessione.  

### Dati di input
* Latitudine $43.963129$ longitudine $10.201176$
* Azimut $-45^\circ$
* Inclinazione rispetto al piano orizzontale $30^\circ$
* Modello **ENEA-SOLTERM**
* Coefficiente di riflessione del suolo $0$

![enea_output](https://user-images.githubusercontent.com/7195133/233844157-f9aecc8c-0561-4ad2-a6f7-3b476e180887.jpg)  

Vediamo allora che nel caso peggiore, quindi a Dicembre, l'irraggiamento richiederebbe l'installazione di un numero di pannelli che il tetto potrebbe non riuscire a sopportare, o comunque risultare in una superficie esagerata. Sappiamo pero' che questa e' una seconda casa di villeggiatura che verra' occupata e/o affittata esclusivamente nei mesi estivi, percio' possiamo permetterci di prendere in considerazione come caso peggiore il mese di Ottobre, che ci offre un irraggiamento di $3.15\ kWh/m^2$ comunque pessimistico rispetto ai mesi estivi, ma che ci permette l'installazione di soli $9$ moduli.  

Calcoliamo la superficie fotovoltaica minima conoscendo il fabbisogno energetico $E_{gior} = 4\ kWh/m^2$ il rendimento totale $\eta_{tot}$ e l'irraggiamento giornaliero medio mensile di $G = 3.15\ kWh/m^2$.  

$E_{gior} = A \cdot G \cdot \eta_{tot} \implies A = \dfrac{E_{gior}}{G \cdot \eta_{tot}} = \dfrac{4}{3.15 \cdot 0.0707} \simeq 18\ m^2$  


## Regolatore di carica  
...

## Sistema di accumulo  
...

## Inverter  
... 

## Schema a blocchi  
...

