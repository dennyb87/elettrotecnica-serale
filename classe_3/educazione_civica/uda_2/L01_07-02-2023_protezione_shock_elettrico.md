# Protezione contro lo shock elettrico  

Lo shock elettrico si ha quando una persona entra in contatto con due parti a potenziale diverso. Si definisce **parte attiva** una parte in tensione in condizioni ordinarie di esercizio e.g. un cavo elettrico. Si parla di:

* **contatto diretto** quando il contatto avviene con una parte attiva
* **contatto indiretto** quando il contatto avviene con una massa a sua volta in contatto con una parte attiva per via di un guasto e.g. l'involucro metallico di un apparecchio

## Protezione contro contatti diretti  

Queste protezioni possono essere:  

* **totali**: isolamento delle parti attive, involucri, o barriere (destinane ai profani e luoghi ordinari)
* **parziali**: ostacoli, distanziamento (destinate e professionisti)

L'**isolamento** ricopre completamente le parti attive ed è rimovibile solo mediante distruzione. Gli involucri o barriere impediscono semplicemente il contatto con le parti attive: la barriera nella direzione abituale di accesso, l'involucro in tutte le direzioni.  

Ai fini della protezione contro i contatti diretti è sufficiente il  grado di protezione **IPXXB**, a maggior ragione il grado di **IP2X**.  

## Protezione contro contatti indiretti  

Queste protezioni possono essere:  

* **attive**: sistemi in grado di togliere tensione e.g. differenziale
* **passive**: sistemi che tendono a limitare la tensione in caso di guasto e.g. doppio isolamento

## Definizioni  

* **massa**: parte conduttrice che puo' andare in tensione a causa di un guasto
* **msolamento funzionale**: isolamento tra le parti attive, e tra queste e la terra, senza questo il funzionamento del componente e' impedito
* **isolamento supplementare**: isolamento aggiuntivo in caso di guasto dell'isolamento principale


# Protezione attiva nel sistema TT

Nei **sistemi TT** (neutro a terra, masse a terra) si devono utilizzare i differenziali, ovvero quei dispositivi in grado di rilevare una differenza di corrente tra fase e neutro.  

![sistema_TT](https://user-images.githubusercontent.com/7195133/219198175-9fef80f0-1d13-4d39-88dc-9ce5e2ff6e3b.jpg)![curva_di_sicurezza](https://user-images.githubusercontent.com/7195133/219171760-68adef17-8b2a-4917-b645-8e0bbad49e98.jpg)  

La curva di sicurezza ci mostra che a $50\ V$ si hanno effetti pericolosi, ma non la fibrillazione ventricolare, percui in condizioni ordinarie si considera una tensione di contatto limite $V_l$ di $50\ V$.  

Per dimensionare l'impianto di terra bisogna allora assicurarsi che la tensione di contatto limite $V_l$ non venga superata, questo dipendera' allora dalla resistenza del dispersore $R_t$ (il terreno), e la corrente di intervento del differenziale $I_{\Delta n}$  

$R_t \cdot I_{\Delta n} \le V_l$  

Diventa evidente che con un differenziale da $30\ mA$ e una resistivita' del suolo di $1000\ \Omega$ potremmo soddisfare la condizione.  

$30 \cdot \cancel{10^{-3}} \cdot \cancel{1000} = 30\ V \le 50\ V$  

Solitamente nei **sistemi TT** si hanno correnti di guasto intorno ai **milliampere** proprio a causa della grande resistivita' del terreno. Diversa la situazione nei **sistemi TN** dove invece si hanno correnti di guasto intorno ai **kiloampere**, vediamo perche'...  

# Protezione attiva nel sistema TN  

Nei **sistemi TN** il neutro e' collegato a terra, e le masse sono collegate al neutro direttamente **TN-C**, oppure tramite un conduttore di protezione **TN-S**.  

![sistema_TN](https://user-images.githubusercontent.com/7195133/219199501-ca3b9dcc-a76b-4e80-8ffd-651e9c50c5c4.jpg)  

Con questo tipo di messa a terra e' evidente che in caso di guasto si presentera' una corrente molto grande, nell'ordine dei kiloampere, quindi paragonabile ad un corto circuito. Questo ci permette di utilizzare anche soltanto un interruttore magnetotermico rendendo differenziale superfluo data la natura delle correnti di guasto.  

![curva_magnetotermico](https://user-images.githubusercontent.com/7195133/219207974-d56fa4e1-9ded-42ea-b231-8db3261d8a7b.jpg)  

