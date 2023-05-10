# Energia solare per uno sviluppo sostenibile  

Le fonti di energia non rinnovabili come gas, petrolio, carbone, sono destinate ad esaurirsi, percio' si vuole sfruttare l'energia solare per uno sviluppo sostenibile.  

> Sostenibile, e' lo sviluppo in grado di soddisfare i bisogni delle generazioni attuali senza compromettere la possibilita' che quelle future riescano a soddisfare i propri.  
> 
> *Gro Harlem Brundtland*

L'energia solare puo' essere sfruttata in due modi:  

* termico
* fotovoltaico

## Fotovoltaico  

L'energia radiante solare viene trasformata in energia elettrica sottoforma di corrente continua, e nel caso opportunamente trasfrormata in alternata all'occorrenza.  

### Vantaggi  

* zero emissioni
* energia gratuita, inesauribile, e presente ovunque
* riduce la dipendenza da combustibili fossili
* costi di esercizio e manutenzione ridotti
* modularita' del sistema
* produzione nel luogo di utilizzo e nelle ore di max. richiesta
* lunga durata dell'impianto

### Svantaggi  

* bassa efficienza 14%-20%
* dipendenza dall'irraggiamento solare, quindi condizioni atmosferiche, posizione geografica etc...
* la disponibilita' non sempre coincide con i fabbisogni e.g. ore notturne
* bassa densita' di potenza con conseguente uso di grandi superfici
* mancanza di standard di progettazione a causa della variabilita' delle caratteristiche in dipendenza della posizione geografica e fabbisogno


## Sistemi grid-connected  

Qui l'energia viene convertita in corrente elettrica alternata ed immessa in rete in parallelo. Puo' eventualmente essere aggiunto un sistema di accumulo per utilizzare l'energia immagazzinata quando i pannelli non producono.  

Il prelievo dell'energia preferisce i pannelli o il sistema di accumulo. Solo nel caso in qui queste fonti non siano disponibili allora si ripiega sulla rete.  

![grid-connected](https://user-images.githubusercontent.com/7195133/234866224-ae361d98-0441-49f1-b756-6e814137426a.jpg)


## Sistemi stand-alone  

Anche detti *a isola* sono sistemi scollegati dalla rete, dove l'energia che alimenta il carico proviene esclusivamente dai pannelli solari o dal sistema di accumulo. Il dimensionamento deve quindi permettere l'alimentazione del carico e la ricarica delle batterie durante le ore di insolazione. Le applicazioni piu' diffuse sono:  

* pompaggio dell'acqua
* ripetitori radio, stazioni metereologiche o sismiche
* sistemi di illuminazione
* segnaletica
* alimentazione dei servizi nei camper o imbarcazioni
* rifugi in alta quota

## Dalla cella al campo fotovoltaico  

![dalla_cella_al_campo_pv](https://user-images.githubusercontent.com/7195133/234900501-4fed6937-cd1a-450d-967a-dffd039d6ddf.jpg)  

## Tipologie di pannelli solari  

I pannelli piu' diffusi sono:  

* monocristallini - alto rendimento > prezzo maggiore
* policristallini - medio rendimento > prezzo contenuto
* a film sottile

Generalmente dimensionati per funzionare a 12V o 24V, in casi particolari anche a 48V.  

## Diodi di bypass  

![bypass_diode](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/6efe6ac2-d848-43f9-8852-f89f25a23d92)  

Il diodo di bypass fa in modo che il pannello (o un gruppo di celle) venga appunto bypassato nei casi in cui questo smette di produrre diventanto un carico con conseguente surriscaldamento e malfunzionamento.  

## Diodi di blocco  

![blocking_diodes](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/d69688f6-ffe6-43fc-98ef-66d65b37751a)  

I diodi di blocco (o anti-inversione) hanno una funzione analoga, ovvero agiscono da "valvola di non ritorno" impedendo l'eventuale ingresso di energia proveniente da altri pannelli per esempio quando i pannelli hanno tensioni diverse.  
