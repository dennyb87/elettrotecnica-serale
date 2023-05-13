# Modelli di diodi  

Per analizzare il comportamento di un circuito reale e' spesso conveniente fare delle semplificazioni, ovvero sostituire i componenti reali con dei componenti equivalenti piu' semplici. Nel caso dei diodi si hanno tre diversi modelli:  

1. modello ideale
2. modello a generatore costante 
3. modello a generatore e resistenza

Avendo gia' preso familiarita' con il modello ideale, passiamo ad esaminare gli altri due modelli osservando la loro curva tensione-corrente e la rappresentazione circuitale.  


## Modello a generatore costante  

![diodo_generatore_costante](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/8b1332fe-8f06-437c-9d2f-31bd17716966)  

In questo modello il diodo in polarizzazione diretta viene rappresentato da un generatore costante, mentre in polarizzazione inversa diventa un circuito aperto.  


## Modello a generatore e resistenza  

![diodo_modello_pratico](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/2e6e87d5-5111-4f7f-a138-c95249cb0495)  

In questo modello il diodo viene sosituito in polarizzazione diretta da un generatore di tensione $U_s$ in serie ad una resistenza $R_f$. E' importante notare che in questo scenario $U_{AK} = R_f \cdot I + U_s$.  

In polarizzazione inversa continuiamo a rappresentarlo come un circuito aperto.  

