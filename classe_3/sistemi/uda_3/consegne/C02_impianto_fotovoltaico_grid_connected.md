# Progetto impianto fotovoltaico grid-connected  

Si vuol progettare un impianto fotovoltaico grid-connected, quindi collegato alla rete di distribuzione, da utilizzare per coprire i fabbisogni di energia elettrica di una utenza domestica ubicata nel comune di Pietrasanta alle coordinate LAT $43.936270$ LONG $10.235543$. Verranno utilizzati moduli fotovoltaici AP-72 Ferrania da 280 W di potenza di picco, installati sul tetto dell'abitazione che si stima avere un'inclinazione di circa $30^\circ$ ed essere orientato approssimativamente a Sud $-10^\circ$ tenendo conto che PGVIS usa come punto cardinale di riferimento il Sud ruotando in senso orario.  

![casa_campagna_60m2](https://user-images.githubusercontent.com/7195133/235432387-5c0158d8-262a-465b-934f-3270359e69bf.jpg)  

![azimuth_approximation_house_60m2](https://user-images.githubusercontent.com/7195133/235432343-78a637f2-f73b-418f-b763-ced900fcb760.jpg)  

## Stima del fabbisogno giornaliero  

![casa_60m2_bolletta](https://user-images.githubusercontent.com/7195133/235434333-82b56cf4-8304-437b-aff4-166e5d15dab5.jpg)  

![consumo_annuo](https://user-images.githubusercontent.com/7195133/235434381-69b17f74-0e95-4328-acff-6fc53be911d3.jpg)  

$\dfrac{1217}{365} \simeq 3.33\ kWh$  

Analizzando la bolletta notiamo che in media si consumano circa $3.33\ kWh$ al giorno. Questo coincide approssimativamente con la mediana mensile dei consumi di circa $100\ kWh$ confermando l'assenza di valori anomali e permettendoci quindi di poter utilizzare $3.33\ kWh$ come fabbisogno giornaliero di riferimento, tenendo in considerazione che essendo grid-connected, potremmo comunque attingere dalla rete in caso di bisogno, o donare il surplus di energia generato nei mesi di massima irradiazione.  

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

Tenendo conto del fatto che e' preferibile l'installazione del numero minimo di pannelli possibile, e come abbiamo gia' accennato, e' sempre possibile attingere alla rete, prendiamo in considerazione $3.33\ kWh$ come fabbisogno giornaliero, e l'irraggiamento nel mese di Dicembre $G = 78.61 / 31 \simeq 2.54\ kWh/m^2$, per trovare il numero di moduli necessari a soddisfare il bisogno energetico.  

