# Contatori in Ladder  

La logica programmata Ladder fornisce l'interfaccia per i contatori. Questi permettono appunto di programmare una commutazione ogni $n$ eventi. Un esempio di applicazione potrebbe essere quella per l'arresto di un nastro trasportatore.  

![contatore_fotocellula_nastro](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7fe479f8-25d3-4b92-b01a-007b5f8d8fc1)  

Il sensore fotocellula e' allora rappresentato da un contatto NO per cui si avra' un segnale logico alto al passaggio di ogni oggetto. Grazie al contatore e' allora possibile arrestare il nastro dopo il passaggio di $n$ oggetti, ad esempio per permetterne l'inscatolamento. Vediamo ora in dettaglio l'interfaccia *counter up* o **CTU**.  

| nome | tipo | descrizione                                                                                                           |
| ---- | ---- | --------------------------------------------------------------------------------------------------------------------- |
| CU   | in   | counter up, nel nostro caso l'ingresso del sensore                                                                    |
| R    | in   | reset                                                                                                                 |
| PV   | in   | preset value, ovvero il valore                   configurato per il quale si vuole eseguire la commutazione in uscita |
| Q    | out  | uscita                                                                                                                |
| CV   | out  | current value, ovvero il valore corrente del contatore                                                                |


![ladder_counter](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/305d14b0-08c1-40a9-8784-4e0ed2987bc3)  


Di seguito un esempio in cui il contatore e' stato configurato con $PV = 3$  

![counter_timeline_example](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/e1469a3d-1ac7-4439-be91-03feb51bd04b)  

Si puo' notare che:  

* ad ogni impulso in ingresso $CU$ il registro interno $CV$ viene incrementato
* quando $CU = PV = 3$ l'uscita $Q$ commuta sullo stato logico alto
* al sengale di reset $R$ il registro viene azzerato e l'uscita $Q$ torna allo stato logico basso