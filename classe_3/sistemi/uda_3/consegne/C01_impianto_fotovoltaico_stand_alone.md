# Progetto impianto fotovoltaico stand-alone  

Si vuol progettare un impianto fotovoltaico stand-alone da installare sul tetto di una seconda casa off-grid di circa $56\ m^2$. L'abitazione e' destinata esclusivamente ad affitti turistici in tarda primavera ed estate, ed e' ubicata in una zona rurale del comune di Pietrasanta alle coordinate LAT $43.963129$ LONG $10.201176$. Si ipotizza un fabbisogno di energia elettrica giornaliero di $4\ kWh$ che tiene conto di un fattore di sicurezza del 20%. Dato il tipo e l'orientamento del tetto si ipotizza un'inclinazione approssimativa di $30^\circ$ ed un angolo di azimuth di $45^\circ$ quindi orientato a Sud-Est tenendo in considerazione che Enea utilizza il punto cardinale Sud come riferimento ruotando in senso antiorario.  

![casa_di_campagna_56m2](https://user-images.githubusercontent.com/7195133/233837334-b19b4d24-239c-408c-8ff1-044e770e394d.jpg)  

![azimuth_approximation](https://user-images.githubusercontent.com/7195133/233838356-4fa0cbcb-190e-4f76-b372-3a99bb5704fa.jpg)  

## Modulo fotovoltaico  

Si vogliono utilizzare moduli **VE172PV-280V** di cui vediamo in tabella le caratteristiche in condizioni standard **STC** ovvero con un irraggiamento di $1000\ W/m^2$, temperatura del modulo di $25^\circ C$, ed un coefficiente di massa d'aria $AM = 1.5$  

| Standard conditions (STC)  |          |            |
| -------------------------- | -------- | ---------- |
| Classe di potenza          | $P_{m}$  | $280\ W$   |
| Efficienza                 | $\eta$   | $14.14$ %  |
| Tensione a circuito aperto | $V_{oc}$ | $45.35\ V$ |
| Corrente di cortocircuito  | $I_{sc}$ | $8.2\ A$   |
| Tensione alla max. potenza | $V_{m}$  | $36.85\ V$ |
| Corrente alla max. potenza | $I_{m}$  | $7.64\ A$  |

| Measures |             |
| -------- | ----------- |
| Length   | $1.98\ m$   |
| Width    | $1\ m$      |
| Area     | $1.98\ m^2$ |
| Weight   | $21.5\ kg$  |

![pv_curve](https://user-images.githubusercontent.com/7195133/233843035-a12080b1-874f-498c-a8bc-0943049679e6.jpg)


## Calcolo moduli per il fabbisogno energetico   

Utilizziamo gli strumenti di calcolo del sito ENEA per stimare l'irraggiamento giornaliero medio mensile nel luogo di installazione. Assumiamo un coefficiente di riflessione pessimistico uguale a zero, anche se tecnicamente con un inclinazione di $30^\circ$ potremmo beneficiare di una piccola riflessione.  

### Dati di input
* Latitudine $43.963129$ longitudine $10.201176$
* Azimut $45^\circ$
* Inclinazione rispetto al piano orizzontale $30^\circ$
* Modello **ENEA-SOLTERM**
* Coefficiente di riflessione del suolo $0$

![enea_output](https://user-images.githubusercontent.com/7195133/233844157-f9aecc8c-0561-4ad2-a6f7-3b476e180887.jpg)  

Vediamo allora che nel caso peggiore, quindi a Dicembre, l'irraggiamento richiederebbe l'installazione di un numero di pannelli che il tetto potrebbe non riuscire a sopportare, o comunque risultare in una superficie esagerata. Sappiamo pero' che questa abitazione verra' occupata e/o affittata esclusivamente intorno ai mesi estivi, percio' possiamo permetterci di prendere in considerazione come caso peggiore il mese di Marzo, che ci offre un irraggiamento di $3.78\ kWh/m^2$ comunque pessimistico rispetto ai mesi estivi, ma che ci permette l'installazione di soli $8$ moduli.  

Calcoliamo ora il numero di moduli/pannelli necessari sapendo che:

* la superficie fotovoltaica minima $A_{f}$ e' il prodotto tra l'area di un pannello $A_p = 1.98\ m^2$ ed il numero $N_p$ di pannelli necessari $A_{f} = A_p \cdot N_p$ 
* il fabbisogno energetico giornaliero $E_{gior} = 4\ kWh/m^2$
* il rendimento totale del sistema $\eta_{s}$ e' il prodotto tra il rendimento del pannello $\eta = 0.1414$ ed il rendimento $\eta_{crai} = 0.5$ di cavi, regolatore di carica, accumulatori, inverter, ovvero $\eta_{s} = \eta_p \cdot \eta_{crai} = 0.1414 \cdot 0.5 = 0.0707$
* l'irraggiamento giornaliero medio in Marzo $G = 3.78\ kWh/m^2$  

$E_{gior} = A_{f} \cdot G \cdot \eta_{s} \implies A_{f} = \dfrac{E_{gior}}{G \cdot \eta_{s}} = \dfrac{4}{3.78 \cdot 0.0707} \simeq 15\ m^2$  

$N_p = \dfrac{A_{f}}{A_{p}} = \dfrac{15}{1.98} \simeq 8$  

Si ha allora che $8$ e' il numero minimo di pannelli per soddisfare il fabbisogno energetico durante la stagione turistica.  

## Sistema di accumulo  

Calcoliamo ora la capacita' $C_{acc}$ del sistema di accumulo, questa terra' conto:

* della energia necessaria per soddifare il fabbisogno energetico $E_{gior}$ che tiene gia' conto di un fattore di sicurezza del 20% per garantire la ricarica degli accumulatori
* del numero $n$ di giorni di autonomia senza ricarica solare
* della percentuale di capacita' effettiva, questo per fare in modo da non scaricare mai completamente le batterie $DOD = 0.8$ *Depth Of Discharge*
* dell'efficienza delle batterie $\eta_{acc}$

Troviamo allora l'energia da immagazzinare nel sistema di accumulo $E_{acc}$  

$E_{acc} = \dfrac{E_{gior} \cdot n}{\eta_{acc} \cdot DOD} = \dfrac{4 \cdot 2}{0.84 \cdot 0.8} \simeq 12\ kWh$  

La capacita' di accumulo e' allora:  

$C_{acc} = \dfrac{E_{acc}}{U_n} = \dfrac{12000}{24} = 500\ Ah$  

Dove $U_n$ e' la tensione nominale degli accumulatori.  

Ci serviranno allora almeno $6$ accumulatori da $12\ V - 200\ Ah$ collegatin in serie-parallelo per ottenere $24\ V\ - 600\ Ah$  

![batteries_parallel](https://user-images.githubusercontent.com/7195133/234634440-c4535491-0d78-48e0-9c07-e5e3b6f6f9de.jpg)  


## Regolatore di carica  

Sceglieremo un regolatore **MPPT** in quanto la tensione $36\ V$ dei pannelli si discosta molto da quella delle batterie, che e' di $24\ V$. Il regolatore dovra' inoltre avere caratteristiche tali da:
* supportare una corrente superiore a quella uscente dai pannelli (con un fattore di sicurezza del 18%) ovvero $7.64 \cdot 8 \cdot 1.18 \simeq 72\ A$
* accettare in ingresso la tensione in uscita dai pannelli, quindi intorno ai $36\ V$

## Inverter  

Scegliamo un inverter leggermente sottodimensionato rispetto alla potenza di picco dell'impianto. In questo caso, essendo la potenza massima di picco $280 \cdot 8 = 2.24\ kW$ si puo' utilizzare un inverter di $2\ kW$ di potenza continuativa e uscita $230\ V\ -\ 50\ Hz$.

## Schema a blocchi  
...

