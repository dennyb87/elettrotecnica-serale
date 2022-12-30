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












