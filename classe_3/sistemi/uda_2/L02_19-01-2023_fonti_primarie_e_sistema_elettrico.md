# Fonti primarie di energia in natura  

Si chiamano **primarie** quelle fonti che possono essere utlizzate con le tecnologie attuali, l'energia elettrica presente in natura, come fulmini ed elettrostatica, non e' una fonte primaria in quanto non siamo (ancora) in grado di sfruttarla.  

Le fonti primarie sono quindi:  

* radiante (sole)
* fluidodinamica (vento, cadute d'acqua, maree)
* chimica (biomasse, combustibili fossili e.g. gas, carbone, petrolio)
* endogena (calore endogeno della terra)
* nucleare (combustibili fissili)

## Vettore energetico  

L'energia elettrica e' un vettore (trasportatore) energetico in quanto si presta ad essere trasportata lontano dalla fonte primaria da cui e' stata generata.  

L'energia delle fonti primarie viene trasformata in energia elettrica per poi essere trasportata e distribuita agli utilizzatori che a loro volta la trasformano di nuovo a seconda delle esigenze e.g. illuminazione, riscaldamento, trasporto, informazione.  


## Conversione di energia idraulica  

![hydropower_plant](https://user-images.githubusercontent.com/7195133/213859722-ef894cf7-dcf4-4c45-940b-3ed3413edd4c.jpg)  

Le centrali che trasformano energia idraulica in elettrica si chiamano centrali idroelettriche. L' energia elettrica viene prodotta da una caduta d'acqua che agisce sulle palette della turbina.  


## Conversione di energia chimica  

![steam_turbine](https://user-images.githubusercontent.com/7195133/213860052-b3e43acc-f911-4215-a0dd-81d9ff53293e.jpg)  

Le centrali che convertono l'energia termica in elettrica sono le centrali termoelettriche o nucleari o
geotermiche. L'energia elettrica viene prodotta grazie alla reazione chimica di un combustibile (carbone, nafta, metano), o dall'energia nucleare, o dall'energia endogena. Il calore fa evaporare l'acqua, e il vapore espandendosi fa girare la turbina.  

# Il sistema elettrico  

Il sistema elettrico e' strutturato in modo da permettere l'alimentazione di un **elevato numero di piccoli apparati utilizzatori** da parte di **pochi generatori di grande taglia**. Assicura l'**autonomia di prelievo**, con **accesso libero** secondo i limiti contrattuali e.g. $3kW$. Permette infine l'**immissione di energia** in rete da parte di tanti **generatori di piccola taglia** e.g. pannelli fotovoltaici domestici.  

![sistema_elettrico](https://user-images.githubusercontent.com/7195133/213861594-bf8a2668-e67e-4583-8942-05e04112eb0d.jpg)  

* centrale
* trasformatore elevatore (alta tensione AT)
* linea alta tensione
* trasformatore media tensione (MT)
* linea media tensione
* cabina di trasformazione (bassa tensione BT)
* linea bassa tensione
* utenze/utilizzatori


```mermaid
flowchart LR
    Generatore-->MT/AT
    MT/AT--"AT 380-220 kV"-->AT/AT
    AT/AT--"AT 150-132 kV"-->AT/MT
    AT/MT--"MT 20-10 kV"-->MT/BT
    MT/BT--"BT 400V(3~)-230V(1~)"-->Utenze
```

## Distribuzione  

La distribuzione avviene prevalentemente in media e bassa tensione, ma in alcuni casi, per alimentare grandi industrie si distribuisce direttamente in alta tensione. La trasformazione in media o bassa viene fatta direttamente sul luogo di utenza.  

## Stazioni e cabine elettriche  

Svolgono almeno una delle seguenti funzioni:  
* trasformazione AT/MT MT/BT MT/AT
* conversione AC/DC DC/AC
* regolazione di tensione, potenza, frequenza, o numero di giri degli alternatori
* smistamento e.g. convogliare piu' linee verso una o piu' linee di partenza

# Punti di forza  

* Flessibilita' di produzione
  * La produzione e' possibile da piu' fonti, e a distanza, quindi puo' essere concentrata in poche grandi centrali.
* Elevanto rendimento in trasmissione e distribuzione
  * La trasmissione e distribuzione di energia elettrica ha un rendimento intorno al 93%
* Praticita' e sicurezza
  * La conversione avviene con sicurezza, pulizia, silenziosita', flessibilita'.  

# Punti di debolezza  

* Perdita di energia
  * Il rendimento globale di un sistema elettrico e' intorno al 35%-45%, e la perdita maggiore avviene nel processo di produzione all'interno delle centrali.
* Equilibrio
  * L'energia elettrica e' accumulabile solo in quantita' limitate, quindi deve essere prodotta nel momento del bisogno e richiede un equilibrio tra produzione e carico.
