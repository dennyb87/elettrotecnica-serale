# UDA 1 – ESERCIZI VACANZE NATALE  
# Parte B  
## Quesito B1  

In una utenza domestica alimentata con una tensione $E = 230V$ risultano accesi i seguenti  
carichi elettrici di cui sono noti:  
1. forno, potenza assorbita $1000W$  
2. frullatore, corrente assorbita $2A$  
3. lampada, resistenza equivalente $529\Omega$  

Sapendo che i carichi sono collegati in parallelo si chiede di trovare:  
* la potenza complessivamente erogata dal generatore  
* la resistenza equivalente del collegamento in parallelo  

## Soluzione  

Essendo i carichi in parallelo significa che ai loro capi c'e' la stessa tensione.  
Possiamo allora grazie alla legge di Ohm trovare le grandezze incognite.  
In particolare ci servono le resistenze che ci permetteranno di trovare $R_{tot}$  
ed infine la potenza totale erogata $P = E \cdot I = E \cdot \dfrac{E}{R_{tot}} = \dfrac{E^2}{R_{tot}}$  

Troviamo quindi la resistenza $R_1$ del forno che assorbe $1000W$  

$P_1 = E \cdot I_1 \implies I_1 = \dfrac{P_1}{E} = 4.35A$  

$I_1 = \dfrac{E}{R_1} \implies \dfrac{E}{I_1} = R_1 = 52.87\Omega$  

La resistenza $R_1$ del forno e' allora di circa $52.87\Omega$  
Troviamo ora la resistenza $R_2$ del frullatore che assorbe $2A$  

$I_2 = \dfrac{E}{R_2} \implies R_2 = \dfrac{E}{I_2} = 115\Omega$  

Non ci resta che calcolare la resistenza totale e quindi la potenza erogata. 

$\dfrac{1}{R_{tot}} = \dfrac{1}{R_1} + \dfrac{1}{R_2} + \dfrac{1}{R_3} = \dfrac{1}{52.87} + \dfrac{1}{115} + \dfrac{1}{529} \simeq 0.0295 \Omega^{-1} \implies R_{tot} = \dfrac{1}{0.0295} \simeq 33.9\Omega$  

$P = E \cdot I = E \cdot \dfrac{E}{R_{tot}} = \dfrac{E^2}{R_{tot}} = \dfrac{230^2}{33.9} \simeq 1560W$  

## QA - Risoluzione circuito elettrico  

![qa_esercizi_natale](https://user-images.githubusercontent.com/7195133/210075396-61068dd7-a771-42c0-8550-e636497135d2.jpg)

Si consideri il circuito in figura, si chiede di:  
1. individuare le correnti elettriche  
2. indicare i punti di connesione semplice e i nodi del circuito  
3. calcolare la resistenza totale del circuito  
4. calcolare la corrente e la potenza erogata dal generatore  
5. stabilire quale resistore assorbe piu' potenza elettrica  

Si hanno quattro punti di connessione di cui due semplici $A, C$ e due nodi $B, D$  

Troviamo prima di tutto $R_{tot}$ per poter derivare quindi $I_1$ e di conseguenza  
le altre correnti, e le altre grandezze incognite.  

$R_s = R_3 + R_4 = 40 + 120 = 160\Omega$  

$R_p = \dfrac{R_2 \cdot R_s}{R_2 + R_s} = \dfrac{40 \cdot 160}{40 + 160} = 32\Omega$  

$R_{tot} = R_1 + R_p = 8 + 32 = 40\Omega$  

$I_1 = \dfrac{E}{R_{tot}} = \dfrac{200}{40} = 5A$  

$I_2 = I_1 \cdot \dfrac{R_s}{R_2 + R_s} = 5 \cdot \dfrac{160}{200} = 5 \cdot 0.8 = 4A$  

$I_3 = I_1 - I_2 = 5 - 4 = 1A$  

$V_{AB} = E \cdot \dfrac{R_1}{R_1 + R_p} = 200 \cdot \dfrac{8}{32} = 50V$    

$V_{BD} = E - V_{AB} = 200 - 50 = 150V$  

$V_{BC} = V_{BD} \cdot \dfrac{R_3}{R_3 + R_4} = 150 \cdot \dfrac{40}{160} = 37.5V$  

$V_{CD} = V_{BD} - V_{BC} = 150 - 37.5 = 112.5V$  


Calcoliamo ora la potenza del generatore e le potenze assorbite.  

$P = E \cdot I_1 = 200 \cdot 5 = 1000W$  
$P_1 = V_{AB} \cdot I_1 = 50 \cdot 5 = 250W$  
$P_2 = V_{BD} \cdot I_2 = 150 \cdot 4 = 600W$  
$P_3 = V_{BC} \cdot I_3 = 37.5 \cdot 1 = 37.5W$  
$P_4 = V_{CD} \cdot I_3 = 112.5 \cdot 1 = 112.5W$  

$P = P_1 + P_2 + P_3 + P_4 = 250 + 600 + 37.5 + 112.5 = 1000W\ verificato\ \checkmark$  

Il resistore che assorbe piu' energia sembra essere $R_2$ con $600W$