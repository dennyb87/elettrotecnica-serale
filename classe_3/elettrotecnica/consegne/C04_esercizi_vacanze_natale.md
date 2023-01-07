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

$V_{AB} = E \cdot \dfrac{R_1}{R_1 + R_p} = 200 \cdot \dfrac{8}{40} = 40V$    

$V_{BD} = E - V_{AB} = 200 - 40 = 160V$  

$V_{BC} = V_{BD} \cdot \dfrac{R_3}{R_3 + R_4} = 160 \cdot \dfrac{40}{160} = 40V$  

$V_{CD} = V_{BD} - V_{BC} = 160 - 40 = 120V$  


Calcoliamo ora la potenza del generatore e le potenze assorbite.  

$P = E \cdot I_1 = 200 \cdot 5 = 1000W$  
$P_1 = V_{AB} \cdot I_1 = 40 \cdot 5 = 200W$  
$P_2 = V_{BD} \cdot I_2 = 160 \cdot 4 = 640W$  
$P_3 = V_{BC} \cdot I_3 = 40 \cdot 1 = 40W$  
$P_4 = V_{CD} \cdot I_3 = 120 \cdot 1 = 120W$  

$P = P_1 + P_2 + P_3 + P_4 = 200 + 640 + 40 + 120 = 1000W\ verificato\ \checkmark$  

Il resistore che assorbe piu' energia sembra essere $R_2$ con $640W$  

## QB - Metodo di Kirchhoff  

Con riferimento al circuito di fig. 1 scrivere il sistema di equazioni che permette  
di risolvere il circuito.  

$$
\begin{cases}
  \begin{aligned}
    I_1 - I_2 - I_3 &= 0 \\
    E - R_1 I_1 - R_2 I_2 &= 0 \\
    R_2 I_2 - R_4 I_3 - R_3 I_3 &= 0 \\
  \end{aligned}
\end{cases}
$$

Sappiamo come visto in passato che con il metodo della sostituizione si puo'  
risolvere il sistema.  

## QC - Teorema di Thevenin  

Il teorema di Thevenin ci dice che un circuito complesso puo' essere visto come  
una black box che rappresente un generatore di tensione $E_{th}$ il quale ha una  
resistenza interna $R_{th}$
Il circuito di fig. 1 sopra, puo' essere allora riscritto in questo modo  
ovviamente omettendo $R_2$

![thevenin_esercizi_natale](https://user-images.githubusercontent.com/7195133/210648618-d39a4473-d697-48fa-8415-ba204173ba4b.jpg)  

Se volessimo allora determinare la corrente che scorre su una resistenza $R_2$ immaginaria  
posta in questo caso tra $B$ e $D$ utilizzando Thevenin dovremmo quindi prima trovare $E_{th}$ e $R_{th}$  

Il generatore di tensione della black box $E_{th}$ non e' altro che la tensione $V_{BD}$  
La tensione $V_{BD}$ deve essere la stessa ai capi di $R_{s} = R_3 + R_4$ che risulta essere:  

$I = \dfrac{E}{R_{tot}}$  

$V_{BD} = R_{s} \cdot I = \dfrac{R_s \cdot E}{R_{tot}} = \dfrac{160 \cdot 200}{168} = 190.48V$  

Una volta trovata la tensione non ci resta che calcolare la resistenza vista dal punto  
di vista del carico o utilizzatore.  

![thevenin_resistance_esercizi_natale](https://user-images.githubusercontent.com/7195133/211064368-8ba55704-b9c1-4bf0-845d-4f5a7c77619d.jpg)  

Si nota allora che da questa prospettiva $R_1$ e' in parallelo con $R_s$  
Troviamo allora la resistenza equivalente $R_{th}$  

$R_{th} = \dfrac{R_1 \cdot R_s}{R_1 + R_s} = \dfrac{8 \cdot 160}{168} = 7.62\Omega$  


Adesso possiamo allora scrivere il circuito equivalente di Thevenin.  

![thevenin_equivalent_esercici_natale](https://user-images.githubusercontent.com/7195133/211066856-3a6b7ea9-7a3d-4bd2-a1d7-21af0cfb32f4.jpg)

La tensione $V_{BC}$ e la corrente che corrente che scorre in $R_2$ sono in perfetto  
accordo con il circuito originale.  

$V_{BC} = E_{th} \cdot \dfrac{R_2}{R_{th} + R_2} = 190.48 \cdot \dfrac{40}{47.62} = 160V$  

$I = \dfrac{V_{BC}}{R_2} = \dfrac{160}{40} = 4A$  

## QD - Principio di sovrapposizione degli effetti  

Si applichi il principio di sovrapposizione degli effetti per determinare la corrente $I_2$  

![qd_pse_fig_2_esercizi_natale](https://user-images.githubusercontent.com/7195133/211146833-ac0cae91-77c0-43bc-863c-4b8d9bdc0d2e.jpg)  

Come gia' sappiamo l'effetto complessivo, in questo caso la corrente $I_2$, in un sistema  
lineare, e' la somma dei singoli effetti $I_2 = I_{2A} + I_{2B}$  
Troviamo allora $I_{2A}$ ovvero la corrente su $R_2$ quando $E_B = 0V$ e resistenza zero.  

$R_{totA} = R_1 + \dfrac{R_2 \cdot R_3}{R_2 + R_3} = 40 + \dfrac{120 \cdot 40}{120 + 40} = 70\Omega$  

$I_{1A} = \dfrac{E_A}{R_{totA}} = \dfrac{140}{70} = 2A$  

$I_{2A} = I_{1A} \cdot \dfrac{R_3}{R_2 + R_3} = 2 \cdot \dfrac{40}{160} = 0.5A$    

Adesso troviamo invece $I_{2B}$ ovvero la corrente su $R_2$ quando $E_A = 0V$ e resistenza zero.  
Notiamo che le resistenze sono speculari percui $R_{tot}$ resta invariata.  

$R_{totA} = R_{totB} = 70\Omega$   

$I_{3B} = \dfrac{E_B}{R_{totB}} = \dfrac{280}{70} = 4A$  

$I_{2B} = I_{3B} \cdot \dfrac{R_1}{R_2 + R_1} = 4 \cdot \dfrac{40}{160} = 1A$  

Si conclude allora che $I_2 = I_{2A} + I_{2B} = 0.5 + 1 = 1.5A$  
