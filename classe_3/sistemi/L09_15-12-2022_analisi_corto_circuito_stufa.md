# Analisi corto circuito di una stufa elettrica  

Ci viene data una stufa elettrica che lavora ad una tensione nominale di $230V$  
consumando $2000W$ di potenza.  

Vogliamo allora calcolare tutte le grandezze elettriche sapendo che la stufa ha una  
resistenza incognita $R_s$ e che viene alimentata in continua da una spina con fase e neutro.

I cavi hanno una lunghezza di $10m$ ed una sezione di $2.5mm^2$.  

![spina_fase_neutro](https://user-images.githubusercontent.com/7195133/209152597-7e2ec853-66bb-490f-af04-3dc72bed446c.jpg)  

Abbiamo ora abbastanza informazioni per poter trovare tutte le grandezze elettriche.  
Avendo una spina con fase $R_f$ e neutro $R_n$ e conoscendo la loro lunghezza possiamo  
calcolarne la resistenza.  

Essendo i cavi uguali possiamo calcolare la resistenza una volta sola $R_e = R_f = R_n$  
utilizziamo quindi la seconda legge di Ohm sapendo che i conduttori sono in rame  
ed hanno quindi un coefficiente di $0.018\Omega\frac{mm^2}{m}$  

$R_e = \rho \cdot \dfrac{\ell}{S} = 0.018 \cdot \dfrac{10}{2.5} = 0.072\Omega$  

Abbiamo appena trovare le resistenze dei conduttori fase e neutro $R_f = R_n = 0.072\Omega$  

Adesso non ci resta che trovare $R_c$ che possiamo derivare una volta trovata la  
resistenza totale $R_{tot}$  

$I = \dfrac{P}{V} = \dfrac{2000}{230} = 8.69A$  

$R_{tot} = \dfrac{E}{I} = \dfrac{230}{8.69} = 26.46\Omega$  

$R_c = R_{tot} - R_f - R_n = R_{tot} - 2R_e = 26.46 - 2 \cdot 0.072 = 26.316\Omega$  

Abbiamo trovato tutte le grandezze elettriche in gioco, adesso non ci resta che simulare  
un corto circuito.   