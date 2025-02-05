# Dimensionamento impianto in media tensione  

Si vuole dimensionare l'impianto dello stabilimento di una cartiera costituito da:

* area $1000\ m^2$ destinata alla lavorazione
* area $250\ m^2$ destinata al magazzino/servizi/mensa
* area $250\ m^2$ destinata agli uffici

## Potenza convenzionale  

Dalla tabella a pagina X-17 del manuale consideriamo $120\ \frac{VA}{m^2}$ per la cartiera, mentre $70 \frac{VA}{m^2}$ per le restanti aree.  

$P_{c1} = 1000\cdot 120 = 12\ kVA$  
$P_{c2} = 250\cdot 70 = 17.5\ kVA$  
$P_{c3} = P_{c2}$  

$S_c = P_{c1}+P_{c2}+P_{c3} = 12+17.5+17.5= 155\ kVA$
$P_c = S_c \cdot \cos\varphi = 155\cdot 0.9 \simeq 140\ kW$  

E' buona norma aggiungere un margine del 30% per potenziali ampliamenti futuri. Questo margine puo' essere aggiunto alla potenza contrattuale $P_c$ oppure come in questo caso, al dimensionamento del trasformatore.  

## Fornitura  

Con una potenza contrattuale $P_c > 100\ kW$ e' necessaria una fornitura in medita tensione (MT) normalmente realizzato con sistema TN (neutro a **T**erra, masse al **N**eutro).  

* tensione di alimentazione $15\ kW$
* neutro compensato
* corrente di guasto a terra $I_f = 40\ A$
* tempo eliminazione guasto $t_f \ge 10\ s$
* corrente cortocircuito trifase massima $I_k = 12.5\ kA$

## Impianto di terra  
