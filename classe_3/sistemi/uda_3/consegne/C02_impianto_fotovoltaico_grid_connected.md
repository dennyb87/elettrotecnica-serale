# Progetto impianto fotovoltaico grid-connected  

Si vuol progettare un impianto fotovoltaico grid-connected, quindi collegato alla rete di distribuzione, da utilizzare per coprire i fabbisogni di energia elettrica di una utenza domestica ubicata nel comune di Pietrasanta alle coordinate LAT $43.936270$ LONG $10.235543$. Verranno utilizzati moduli fotovoltaici AP-72 Ferrania da 280 W di potenza di picco, installati sul tetto dell'abitazione che si stima avere un'inclinazione di circa $30^\circ$ ed essere orientato approssimativamente a Sud $-10^\circ$ tenendo conto che PGVIS usa come punto cardinale di riferimento il Sud ruotando in senso orario.  

![casa_campagna_60m2](https://user-images.githubusercontent.com/7195133/235432387-5c0158d8-262a-465b-934f-3270359e69bf.jpg)

![azimuth_approximation_house_60m2](https://user-images.githubusercontent.com/7195133/235432343-78a637f2-f73b-418f-b763-ced900fcb760.jpg)

## Stima del fabbisogno giornaliero  

![casa_60m2_bolletta](https://user-images.githubusercontent.com/7195133/235434333-82b56cf4-8304-437b-aff4-166e5d15dab5.jpg)  

![consumo_annuo](https://user-images.githubusercontent.com/7195133/235434381-69b17f74-0e95-4328-acff-6fc53be911d3.jpg)  

$\dfrac{1217}{365} \simeq 3.33\ kWh$  

Analizzando la bolletta notiamo che in media si consumano circa $3.33\ kWh$ al giorno. Questo coincide approssimativamente con la mediana mensile dei consumi di circa $100\ kWh$ confermando l'assenza di valori anomali e permettendoci quindi di poter utilizzare $3.33\ kWh$ come fabbisogno giornaliero di riferimento, tenendo in considerazione che essendo grid-connected, potremmo comunque attingere dalla rate in caso di bisgno, o donare il surplus di energia generato nei mesi di massima irradiazione.  

