# Breadboard  

![breadboard_circuito_semplice](https://user-images.githubusercontent.com/7195133/196028100-0553480c-b259-440b-8f4f-c6d163afdf5b.jpg)![breadboard_connections](https://user-images.githubusercontent.com/7195133/196026839-f31075e7-812c-4de5-89e0-d7ce8949e8b5.jpg)  

In italiano è talvolta chiamata **basetta sperimentale** o **basetta di prova**, è uno strumento utilizzato  
per creare prototipi di circuiti elettrici che non richiede saldature ed è completamente riutilizzabile.  
L'immagine a destra evidenzia la struttura dei collegamenti.  


# Misure elettriche  

Per risolvere un circuito si hanno a disposizione due tipi di valori: **nominali**, e **misurati**.  
Si consiglia di eseguire i calcoli con entrambe per accertarsi che i valori misurati siano in accordo  
con quelli nominali e evidenziare eventuali errori.  
Si trovano quindi prima i valori delle resistenze utilizzando il **codice a colori**, successivamente si misurano i resistori con il multimetro.  

# Codice a colori  

![codice_a_colori_resistori](https://user-images.githubusercontent.com/7195133/196046789-fbf1d8d7-1468-4e3a-8cb8-8be571efcf4c.jpg)  

Per esempio il resistore in figura si calcola estraendo i numeri associati alle bande di colore.  

 |banda 1|banda 2|moltiplicatore|tolleranza|
 |--|--|--|--|
 |$\color{red}rosso$|$\color{purple}viola$|$\color{green}verde$|$\color{orange}oro$|
 |2|7|$10^5$|$\pm 5$%|  

Quindi il resitore in figura ha una resistenza di $27 \cdot 10^5 \Omega \pm 5$% $= 2700000 \Omega \pm 5$% $= 2.7 M\Omega \pm 5$%  


# Valori commerciali dei resistori

I resistori vengono fabbricati e commerciati con valori standard, quindi si puo' sempre controllorare che il valore calcolato (e/o misurato) sia in accordo con questi.  

![valori_commerciali_resistori](https://user-images.githubusercontent.com/7195133/196048416-761a0bc3-6dca-4a66-b0ca-a52ac67d6d71.jpg)  

E' importante notare che i valori aumentano in potenze di 10 da sinistra verso destra e.g. $10^0$ $10^1$ $10^2$ e cosi' via.  
