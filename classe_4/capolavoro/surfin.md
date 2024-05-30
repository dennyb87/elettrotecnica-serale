# Surfin  

Trovo particolarmente affascinante la scoperta di patterns, cosi' come il potere predittivo che nasce ogni volta che le relazioni tra entita' vengono in qualche modo rivelate. Questa voglia di osservare e di creare mi ha spinto a cercare un passatempo che mi permetta di approfondire i miei interessi e al tempo stesso acquisire nuove abilita' da impiegare anche a livello lavorativo. Cosi' per poter sperimentare nelle dimensioni tech, surf e analisi dati, ho deciso di creare un'applicazione web che ho chiamato *"surfin"*.  

L'idea e' quella di utilizzare API di terze parti per:

1. presentare dati atmosferici e marini in real-time negli spot surfistici
2. raccogliere dati in modo periodico per poterli analizzare e potenzialmente fornire un servizio di *surf-alert*

## API dati atmosferici e marini  

Facendo qualche ricerca online ho inizialmente selezionato:  

1. [meteonetwork.it](https://www.meteonetwork.it/supporto/meteonetwork-api/) - espone gratuitamente i dati real-time di un elevato numero di stazioni meteo sul territorio italiano
2. [windy webcams](https://api.windy.com/webcams/api/v3/docs) - espone gratuitamente le immagini di numerose webcam
3. [ispra dataset ron](https://dati.isprambiente.it/dataset/ron/) - attualmente interrotta per manutenzione, ma altrimenti espone gratuitamente dati marini real-time provenienti da boe ondametriche direzionali

Tutte le sorgenti soddisfano i requisiti minimi necessari, ovvero espongono i dati in modo grauito e i permmettono il loro processamento e presentazione.  

## Piattaforma di lancio  

Dopo qualche ricerca ho deciso di utilizzare [Oracle Cloud Infrastructure](https://www.oracle.com/cloud/) in quanto mi permette di lanciare l'istanza di un server remoto in modo completamente gratuito grazie al loro [free tier](https://www.oracle.com/cloud/free/). Questo e' particolarmente vantaggioso in quanto si ha il pieno controllo via `ssh` del server remoto, caratteristica che apre la strada a svariate possibilita lato backend.  

\pagebreak  

## Demo page  

Al momento esiste una pagina dimostrativa all'indirizzo [https://surfin.duckdns.org](https://surfin.duckdns.org/) dove logo e design sono stati realizzati con [InkScape](https://en.wikipedia.org/wiki/Inkscape). La parte piu' problematica e' stato il deployment non essendo particolarmente familiare con l'infrastruttura Oracle, ma sono comunque riuscito a scrivere una [guida passo-passo](https://github.com/dennyb87/my-oci-utils/blob/main/deploy/django.md) che ho reso pubblica.  

### Repositories  

* demo app > [surfin](https://github.com/dennyb87/surfin)
* guida al deployment su Oracle > [my-oci-utils](https://github.com/dennyb87/my-oci-utils)
* client meteonetwork > [meteonetwork-api-client-python](https://github.com/dennyb87/meteonetwork-api-client-python)
* client windy-webcams > [windy-webcams-api-client-python](https://github.com/dennyb87/windy-webcams-api-client-python)
