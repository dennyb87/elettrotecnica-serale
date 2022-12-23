# Analisi corto circuito di una stufa elettrica  

Ci viene data una stufa elettrica che lavora ad una tensione nominale di $230V$  
consumando $2000W$ di potenza.  

Vogliamo allora calcolare tutte le grandezze elettriche sapendo che la stufa ha una  
resistenza incognita $R_s$ e che viene alimentata in continua da una spina con fase e neutro.

I cavi hanno una lunghezza di $10m$ ed una sezione di $2.5mm^2$.  

![spina_fase_neutro](https://user-images.githubusercontent.com/7195133/209152597-7e2ec853-66bb-490f-af04-3dc72bed446c.jpg)![stufa_elettrica](https://user-images.githubusercontent.com/7195133/209300081-15c3f656-ed04-4476-b32c-5ba4eb2c8d3b.jpg)  

Abbiamo ora abbastanza informazioni per poter trovare tutte le grandezze elettriche.  
Avendo una spina con fase $R_f$ e neutro $R_n$ e conoscendo la loro lunghezza possiamo  
calcolarne la resistenza.  

Essendo i cavi uguali possiamo calcolare la resistenza una volta sola $R_e = R_f = R_n$  
utilizziamo quindi la seconda legge di Ohm sapendo che i conduttori sono in rame  
ed hanno quindi un coefficiente di resistivita' di $0.018\Omega\frac{mm^2}{m}$  

$R_e = \rho \cdot \dfrac{\ell}{S} = 0.018 \cdot \dfrac{10}{2.5} = 0.072\Omega$  

Abbiamo appena trovare le resistenze dei conduttori fase e neutro $R_f = R_n = 0.072\Omega$  

Adesso non ci resta che trovare $R_s$ che possiamo derivare una volta trovata la  
resistenza totale $R_{tot}$  

$I = \dfrac{P}{V} = \dfrac{2000}{230} = 8.69A$  

$R_{tot} = \dfrac{E}{I} = \dfrac{230}{8.69} = 26.46\Omega$  

$R_s = R_{tot} - R_f - R_n = R_{tot} - 2R_e = 26.46 - 2 \cdot 0.072 = 26.316\Omega$  


Abbiamo trovato tutte le grandezze elettriche in gioco, e lo schema in condizioni  
di normale funzionamento appare come segue.  

![schema_stufa_elettrica](https://user-images.githubusercontent.com/7195133/209301107-dd62cd85-29c7-482a-8d0d-0cbbc76f34c6.jpg)  

Adesso non ci resta che simulare un corto circuito.  
Nel caso in cui il conduttore di fase trovasse una strada alternativa per unirsi  
al neutro senza passare da $R_s$ allora si avrebbe una situazione come in figura.  

![schema_corto_circuito_stufa](https://user-images.githubusercontent.com/7195133/209302073-38c36147-a8ff-4a9e-b0d4-eacb04c87bd9.jpg)  

Le cariche allora tenderanno a passare dal percorso con meno resistenza  
$R_s$ verra' quindi ignorata e la resistenza vista dal generatore sara' quindi $2R_e$  
che come abbiamo visto e' molto piccola.  

Calcoliamo ora la corrente che si verrebbe a creare.  

$R_{tot} = 2R_e = 2 \cdot 0.072 = 0.144\Omega$  

$I = \dfrac{E}{R_{tot}} = \dfrac{230}{0.144} = 1597.22A$  


In caso di corto circuito si avrebbe quindi un enorme corrente di $1597.22A$ con  
conseguenti danni.
