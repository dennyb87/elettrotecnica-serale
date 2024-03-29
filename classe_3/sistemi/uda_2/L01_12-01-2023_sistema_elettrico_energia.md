# Sistema elettrico per l'energia  

Con sistema elettrico per l'energia si intende quindi l'insieme di elementi ed infrastrutture che rendono possibile la **produzione**, **trasmissione**, **distribuzione**, **utilizzo**, e **dispacciamento** dell'energia elettrica, e del modo in cui interagiscono tra loro.  


## Terna  

Terna è una società italiana operatrice delle reti di trasmissione dell'energia elettrica, occupa la posizione centrale nella filiera: sono responsabili della trasmissione, ossia la gestione, il mantenimento e lo sviluppo della rete elettrica nazionale ad alta tensione, e del dispacciamento.  

Qui un'animazione di [Terna](https://www.terna.it/it/sistema-elettrico/ruolo-terna/come-funziona-sistema-elettrico) sul funzionamento del sistema elettrico: in verde i flussi elettrici, in giallo i flussi di dati. 


![terna_electric_system](https://user-images.githubusercontent.com/7195133/212567924-c8c3c74d-140b-44d6-b166-aed87f67dd60.gif)  


## Produzione  

Con produzione sin intende la trasformazione di un certo tipo di energia in energia elettrica:
* idrico
* gas / carbone
* geotermico / eolico / biomasse / fotovoltaico
* import / export

Il mercato della produzione e' completamente liberalizzato. 

## Trasmissione  

Per trasmissione si intende la trasmissione di grandi quantita' di energia su lunghe distanze, quindi attraverso tralicci su tutto il territorio, ovvero la cosiddetta **rete elettrica nazionale**.  
Si trasmette in alta tensione per tenere bassa la corrente che altrimenti scalderebbe i cavi dissipando potenza, senza contare che servirebbero cavi di sezione molto grande per permettere correnti di una certa entita', per cui si preferisce alta tensione e bassa corrente.     

## Distribuzione  

Con distribuzione si intende le modalita' con cui l'energia viene appunto distribuita agli utenti, qunidi si tratta di piccole distanze e piccole quantita' di energia.  

## Utenze  

Per utenze si intende qualunque modo in cui l'energia viene utilizzata, e quindi di nuovo trasformata in luce, calore, movimento, informazione e.g. illuminazione, riscaldamento, motori, computer.  

## Dispacciamento  

Il dispacciamento e' l'attività che consiste nel gestire i flussi di elettricità sulla rete in qualsiasi momento. E' quindi il sistema di controllo che in base ai feedback delle utenze, produzione, e trasmissione, cerca di mantenere l'equilibrio tra domanda ed offerta di energia.  

Questo e' molto importante perche' **l'energia non puo' essere immagazzinata**, deve quindi essere prodotta nel momento del bisogno, e se la domanda supera l'offerta significa che acluni utenti rimarranno a bocca asciutta, ovvero un blackout.  

Se invece si produce piu energia di quanta ne serva si otterra' un aumento della frequenza nella rete causando il malfunzionamento e consequente disconnessione degli apparati che non la supportanto. La frequenza viene in effetti utilizzata come indicatore per l'autoregolazione.  


# Diagramma di carico e forecasting  

Si definisce **diagramma di carico** la curva della potenza attiva prelevata dall'utenza in funzione del tempo. La produzione viene stimata attraverso l'analisi di dati giorno per giorno in quanto non e' possibile fare previsioni accurate a lungo termine (vedi [grafico interattivo](https://www.terna.it/it/sistema-elettrico/transparency-report/total-load)).  

![total_load](https://user-images.githubusercontent.com/7195133/213254533-45f607a7-8a3e-4d10-937a-8a90fb851954.jpg)  

Si ha il tempo in ore sull'asse delle ascisse, e la potenza in gigawatt sull'asse delle ordinate. L'area sotto la curva blu rappresenta quindi l'energia totale effettivamente consumata, $724.5\ GWh$ (gigawatt-ora) in questo caso. Dato che l'energia viene prodotta nel momento del bisogno si ha uguaglianza tra l'energia prodotta e quella utilizzata.  
