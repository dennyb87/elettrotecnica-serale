# Campo elettrico e condensatori  

>### 1. Indica quali sono i rispettivi simboli del campo elettrico e della sua unita' di misura

Del campo elettrico viene misurata la sua *intensita'* $K$ che e' definita come la tensione $U$ per unita' di distanza $d$, per definizione il metro, la sua unita' di misura e' quindi volt su metro $V/m$.  

$K = \dfrac{U}{d}$  

#
>### 2. Qual e' il verso che viene convenzionalmente attribuito alle linee di forza del campo elettrico ?  

Per convenzione si utilizza il verso del moto di una carica campione positiva, che e' anche il verso della forza a cui e' soggetta, lasciata libera di muoversi in un campo elettrico, quindi sempre da un polo positivo ad un polo negativo.  

#
>### 3. Qual e' l'unita' di misura della capacita' di un condensatore ?  

L'unita' di misura della capacita' di un condensatore e' il *farad* (simbolo $F$).  

#
>### 4 Come sono indicate rispettivamente le quantita' di carica sulle armature di un condensatore e la sua unita' di misura ?  

La quantita' di carica si indica con $Q$ e la sua unita' di misura e' il *coulomb* (simbolo $C$).  

#
>### 5. A quanti $uF$ corrispondono rispettivamente $12\ pF$ e $10\ nF$ ?  

$12\ pF = 12 \cdot 10^{-12}\ F = 12 \cdot 10^{-6} \cdot 10^{-6}\ F = 0.000012\ \mu F$  
$10\ nF = 10 \cdot 10^{-9}\ F = 10 \cdot 10^{-3} \cdot 10^{-6}\ F = 0.01\ \mu F$  

#
>### 6. Scrivi la relazione che esiste tra capacita', carica e tensione in un condensatore.  

Esiste una relazione lineare in quanto all'aumentare della tensione si ha un aumento di carica, per cui la capacita' risulta costante, la quale non dipende da queste grandezze ma e' in effetti una proprieta' del condensatore esaminato.   

$C = \dfrac{Q}{V}$  

Da cui si ha anche che $Q = C \cdot V$ oppure $V = \dfrac{Q}{C}$  

#
>### 7. Qual e' la funzione caratteristica di un condensatore ?  

Il condensatore e' sostanzialmente un dispositivo che ci permette di immagazzinare cariche elettriche.  

#
>### 8. Un sistema e' composto da quattro conduttori isolati. Quante capacita' parziali fra di essi si possono considerare ?  

La domanda e' ambigua in quanto non ci da abbastanza informazioni per capire la geometria del sistema. Tuttavia supponendo che si tratti di quattro conduttori in serie, possiamo immaginare un sistema di tre condensatori che rappresentano le capacita' tra $4$ conduttori isolati.  

![sistema_4_conduttori_isolati](https://user-images.githubusercontent.com/7195133/215318793-4f27f5c0-4cf5-484d-bcb2-2fda5f9a5d5f.jpg)  

Possiamo allora concludere che esistono $6$ capacita' parziali ovvero $C_1, C_2, C_3, C_{12}, C_{23}, C_{13}$  

$C_{12} = \dfrac{C_1 \cdot C_2}{C_1 + C_2}$  

$C_{23} = \dfrac{C_2 \cdot C_3}{C_2 + C_3}$  

$C_{13} = \dfrac{C_1 \cdot C_3}{C_1 + C_3}$  

Mentre la capacita' totale puo' essere trovata con:  

$C_{tot} = \dfrac{C_1 \cdot C_{23}}{C_1 + C_{23}} = \dfrac{C_2 \cdot C_{13}}{C_2 + C_{13}} = \dfrac{C_3 \cdot C_{12}}{C_3 + C_{12}}$  

#
>### 9. Un condensatore di $10\ \mu F$ ha una tensione pari a $100\ V$ ai suoi capi. Calcola la carica che vi e' immagazzinata.  

$Q = C \cdot V = 10 \cdot 10^{-6} \cdot 10^2 = 10 \cdot 10^{-4} = 0.001\ C = 1\ mC$  

#
>### 10. Solo uno dei seguenti fattori influenza la capacita' di un condensatore. Indica quale:  

* [x] spessore del dielettrico
* [ ] resistenza delle armature
* [ ] tensione di lavoro
* [ ] tensione di rottura

Sappiamo che la capacita' dipende dalla geometria del condensatore e dal materiale del dielettrico. Lo spessore del dielettrico determina la distanza tra le armature, ragion per cui e' un fattore che certamente influenza la sua capacita'.  

#
>### 11. Un condensatore da $330\ pF$ usa un dielettrico con permittivita' relativa di $2.2$. Determina il nuovo valore che avra' la capacita' incrementando il valore della permittivita relativa a $6.6$  

$C = \varepsilon_{r1} \cdot \varepsilon_0 \cdot \dfrac{S}{d}$  

Trovando il rapporto di incremento ovvero $r = \dfrac{6.6}{2.2} = 3$ si ha che con la nuova permittivita' relativa la capacita' diventa di $330 \cdot 10^{-12} \cdot 3 = 990 \cdot 10^{-12} = 990\ pF$  
Dimostrato dal fatto che $\dfrac{C}{\varepsilon_{r1}\varepsilon_0} = \dfrac{S}{d} \implies \varepsilon_{r2} \cdot \varepsilon_0 \cdot \dfrac{C}{\varepsilon_{r1}\varepsilon_0} = 6.6 \cdot \varepsilon_0 \cdot \dfrac{330 \cdot 10^{-12}}{2.2 \cdot \varepsilon_0} = 3 \cdot 330 \cdot 10^{-12}= 990\ pF$  

#
>### 12. Un condensatore ad armature con facce piane e parallele ha una capacita' di $100\ nF$. Determina il nuovo valore della capacita' nel caso in cui l'area delle armature sia raddoppiata e la distanza tra di esse sia dimezzata.  

Sapendo che $\dfrac{2a}{\frac{b}{2}} = 2a \cdot\dfrac{2}{b} = 2 \cdot 2 \cdot \dfrac{a}{b} = 4 \cdot \dfrac{a}{b}$  

Possiamo concludere che la capacita' sia quadruplicata $4 \cdot 100 \cdot 10^{-9} = 400\ nF$  
