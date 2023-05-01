# Progetto impianto fotovoltaico grid-connected  

Si vuol progettare un impianto fotovoltaico grid-connected, quindi collegato alla rete di distribuzione, da utilizzare per coprire i fabbisogni di energia elettrica di una utenza domestica ubicata nel comune di Pietrasanta alle coordinate LAT $43.936270$ LONG $10.235543$. Verranno utilizzati moduli fotovoltaici AP-72 Ferrania da 280 W di potenza di picco, installati sul tetto dell'abitazione che si stima avere un'inclinazione di circa $30^\circ$ ed essere orientato approssimativamente a Sud $-10^\circ$ tenendo conto che PGVIS usa come punto cardinale di riferimento il Sud ruotando in senso orario.  

![casa_campagna_60m2](https://user-images.githubusercontent.com/7195133/235432387-5c0158d8-262a-465b-934f-3270359e69bf.jpg)  

![azimuth_approximation_house_60m2](https://user-images.githubusercontent.com/7195133/235432343-78a637f2-f73b-418f-b763-ced900fcb760.jpg)  

## Dati di targa AP-72 Ferrania 280W  

| Standard conditions (STC)  |          |            |
| -------------------------- | -------- | ---------- |
| Classe di potenza          | $P_{m}$  | $280\ W$   |
| Efficienza                 | $\eta$   | $14.18$ %  |
| Tensione a circuito aperto | $V_{oc}$ | $45.35\ V$ |
| Corrente di cortocircuito  | $I_{sc}$ | $8.4\ A$   |
| Tensione alla max. potenza | $V_{m}$  | $35.40\ V$ |
| Corrente alla max. potenza | $I_{m}$  | $7.9\ A$   |

| Measures |             |
| -------- | ----------- |
| Length   | $1.977\ m$  |
| Width    | $0.996\ m$  |
| Area     | $1.97\ m^2$ |
| Weight   | $21.5\ kg$  |


## Stima del fabbisogno giornaliero  

![casa_60m2_bolletta](https://user-images.githubusercontent.com/7195133/235434333-82b56cf4-8304-437b-aff4-166e5d15dab5.jpg)  

![consumo_annuo](https://user-images.githubusercontent.com/7195133/235434381-69b17f74-0e95-4328-acff-6fc53be911d3.jpg)  

$\dfrac{1217}{365} \simeq 3.33\ kWh$  

Analizzando la bolletta notiamo che in media si consumano circa $3.33\ kWh$ al giorno, ma nel mese di Dicembre si ha il consumo massimo di circa $125\ kWh$. Allora troviamo il fabbisogno giornaliero di riferimento $E_{gior} = \dfrac{125}{31} \simeq 4\ kWh$, tenendo in considerazione che essendo grid-connected, potremmo comunque attingere dalla rete in caso di bisogno, o donare il surplus di energia generato nei mesi di massima irradiazione.  

## Stima irraggiamento e produzione annua con PVGIS  

Attraverso PVGIS vogliamo stimare l'irraggiamento e la produzione con un modulo **AP-72 Ferrania** da $280\ W$ di picco in **STC**. Si ipotizzano:  

* $\eta_m = 0.1418$ l'efficienza del modulo  
* $\eta_i = 0.92$ l'efficienza dell'inverter  
* $\eta_c = 0.99$ l'efficienza dei cavi  
* $\eta_{ps} = 0.8$ l'efficienza dei contatori di produzione/scambio  

$\eta_{tot} = \eta_m \cdot \eta_i \cdot \eta_c \cdot \eta_{ps} = 0.1418 \cdot 0.92 \cdot 0.99 \cdot 0.8 \simeq 0.1$  

Dati di input:  

* potenza di picco $280\ W$ in **STC**
* efficienza $\eta_{tot}$ del 10%
* inclinazione tetto $30^\circ$
* azimuth $-10^\circ$

![pvgis_input](https://user-images.githubusercontent.com/7195133/235484272-e75851bf-485a-4ba6-b829-31968ab8d638.jpg)  

![pvgis_production](https://user-images.githubusercontent.com/7195133/235485245-7b11be1d-2039-46c9-b0de-9abe240b7c74.jpg)  

![pvgis_radiation](https://user-images.githubusercontent.com/7195133/235485317-924099fe-7e9d-4ba4-b645-ac82f674bf1c.jpg)

Si ha allora che con un modulo/pannello si otterrebbe una produzione annua di circa $389.34\ kWh$ che sappiamo non essere sufficienti per coprire il fabbisogno annuale dell'utenza di circa $1217\ kWh$.  

## Calcolo numero di moduli  

Tenendo conto del fatto che e' preferibile l'installazione del numero minimo di pannelli possibile, e come abbiamo gia' accennato, e' sempre possibile attingere alla rete, prendiamo in considerazione $E_{gior} = 4\ kWh$ come fabbisogno giornaliero, e l'irraggiamento nel mese di Dicembre $G = 78.61 / 31 \simeq 2.54\ kWh/m^2$, per trovare il numero di moduli necessari a soddisfare il bisogno energetico.  

$E_{gior} = A_{f} \cdot G \cdot \eta_{tot} \implies A_{f} = \dfrac{E_{gior}}{G \cdot \eta_{tot}} = \dfrac{4}{2.54 \cdot 0.1} \simeq 15.75\ m^2$  

$N_p = \dfrac{A_{f}}{A_{p}} = \dfrac{15.75}{1.97} \simeq 8$  

Si ha allora che $8$ e' il numero minimo di pannelli per soddisfare il fabbisogno energetico.  

Dove:  

* la superficie fotovoltaica minima $A_{f}$ e' il prodotto tra l'area di un pannello $A_p = 1.97\ m^2$ ed il numero $N_p$ di pannelli necessari $A_{f} = A_p \cdot N_p$ 
* $\eta_{tot}$ e' l'efficienza dell'intero sistema


## Schema a blocchi  

Da sinistra verso destra si hanno:  

* pannelli fotovoltaici
* inverter
* contatore di produzione
* contatore di scambio

![grid_connected_block_diagram](https://user-images.githubusercontent.com/7195133/235495596-f947f8a2-f589-4247-948e-174a2fae8fc8.jpg)  


## Valutazione del rendimento  

L'impianto cosi' progettato permetterebbe di soddisfare il fabbisogno energetico solo nel caso in cui l'energia venisse consumata durante le ore diurne. Ma sappiamo che realisticamente una normale utenza domestica e' caratterizzata da un fabisogno energietico che si estende alle ore notture, e al mattino presto. Allora senza sistema di accumulo, si dovra' sfruttare l'energia della rete, portando di conseguenza ad avere dei costi che difficilmente saranno compensati dal surplus di energia scambiata durante le ore diurne.  