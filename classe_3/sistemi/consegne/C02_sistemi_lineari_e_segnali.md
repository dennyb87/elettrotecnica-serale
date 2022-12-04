# UDA 1 - SISTEMI LINEARI E SEGNALI  

## Q1 - Riduttore di tensione  

![uda1_sistemi_lineari_e_segnali_fig1](https://user-images.githubusercontent.com/7195133/205484810-2b572772-9ad7-4d78-94cb-9e714db6fa96.jpg)  

Calcolare la funzione di trasferimento del seguente sistema sapendo che  

$R_1 = 20\Omega$  
$R_2 = 10\Omega$  
$R_3 = 30\Omega$  
$R_4 = 45\Omega$  

Completare quindi la tabella mostrata in figura.  

## Soluzione  

Sappiamo che la funzione di trasferimento e' uguale alla formula del partitore  
di tensione. Per completare la tabella pero' abbiamo bisogno di semplificare  
il circuito trovando la resistenza equivalente delle resistenze in serie e in parallelo.  

$R_s = R_1 + R_2 = 20 + 10 = 30\Omega$  
$R_{eq} = \frac{R_3 \cdot R_s}{R_3 + R_s}$  

Ma $R_3 = R_s = R$ allora...  

$R_{eq} = \frac{R*R}{R+R} = \frac{R^2}{2R} = \frac{R}{2} = \frac{30}{2} = 15\Omega$  

Adesso sapendo che $V_2 = \frac{R_4}{R_4 + R_{eq}} \cdot V_1$ si nota immediatamente che  
la funzione di trasferimento e' $F = \frac{R_4}{R_4 + R_{eq}} = \frac{45}{60} = \frac{3}{4}$ quindi  

$V_2 = F \cdot V_1 = \frac{3}{4} \cdot V_1$  

Allora possiamo risolvere trovando $V_1$ moltiplicando entrambe i termini  
dell'equazione per il reciproco di $F$ ovvero $\frac{1}{F} = \frac{R_4 + R_{eq}}{R_4} = \frac{4}{3}$. 

$V_1 = \frac{R_4 + R_{eq}}{R_4} \cdot V_2 = \frac{4}{3} \cdot V_2$  

Possiamo ora completare la tabella.  

| $V_1\ [V]$ | $V_2\ [V]$ |
| ---------- | ---------- |
| $0$        | $0$        |
| $100$      | $75$       |
| $-100$     | $-75$      |
| $20$       | $15$       |
| $30$       | $22.5$     |


## Q2 - Lettura grafico  
### Calcolo del valore medio temporale e della velocità di variazione nel tempo  

![uda1_sistemi_lineari_e_segnali_fig2](https://user-images.githubusercontent.com/7195133/205486938-efeec72a-9999-4609-8e36-0ab9561d0f7e.jpg)  

Per ciascuno dei seguenti grafici valutare il tempo di osservazione, il valore   
minimo, il valore massimo, il valore medio del segnale nel tempo di osservazione,  
la velocità di variazione nel tempo, stimare (utilizzando il grafico) il valore  
all’istante $t = 70s$  


## Soluzione grafico $a(t)$  

Per semplicita' poniamo $y = a(t)$

$t_{oss} = 120s$  
$y_{max} = 50$  
$y_{min} = 0$  
$A_1 = b \cdot a = 60 \cdot 50 = 3000$    
$A_2 = \frac{b \cdot a}{2} = \frac{60 \cdot 50}{2} = \frac{A_1}{2}= 1500$  
$y_{medio} = \frac{A_1 + A_2}{t_{oss}} = \frac{3000+1500}{120} = 37.5$  

Come si vede in figura $y$ rimane costante fino a $t = 60s$, la velocita' di  
variazione e' quindi di $0$ al secondo.  
Calcoliamo invece da $t > 60s$ a $t = 120s$ chiamando $v$ il rapporto tra  
variazione di $y$ e variazione di $t$

$v = \frac{\Delta{y}}{\Delta{t}} = \frac{0 - 50}{120 - 60} =  - \frac{5}{6}$  

Questo significa che si ha una variazione di circa $-0.83$ al secondo quando $t > 60s$.  
Adesso possiamo trovare il valore all'istante $t = 70s$ sapendo che c'e' una  
variazione di $-0.83$ al secondo negli ultimi $10$ secondi.  
Allora $y$ al tempo $t = 70s$ sara'...

$y = a(70) = 50 + 10 \cdot - \frac{5}{6} = 41.67$  

Per trovare invece la velocita' di variazione nel tempo media, possiamo allora  
trovare la differenza di valore durante il tempo di osservazione.

$v_{medio} = \frac{0 -50}{120} = -0.42$  

Si ha quindi una variazione media di $-0.42$ al secondo.  

## Soluzione grafico $b(t)$  

Per semplicita' poniamo $y = b(t)$  

$t_{oss} = 100s$  
$y_{max} = 100$  
$y_{min} = -60$  
$A_1 = b \cdot a = 60 \cdot 100 = 6000$  
$A_2 = b \cdot a = 40 \cdot -60 = -2400$  
$y_{medio} = \frac{A_1 + A_2}{t_{oss}} = \frac{6000-2400}{100} = 36$  

In questo caso abbiamo due valori costanti di $y$ rispettivamente  

$y_{max} = 100$  
$y_{min} = -60$  

Allora per trovare $y$ al tempo $t = 70s$ ci basta controllare se $y$ al tempo $t$ 
si trova al punto minimo o massimo.  
Si vede immediatamente che $y$ al tempo $t = 70s$ e' al suo minimo, quindi sara' $b(70) = -60$  

Per trovare invece la velocita' di variazione nel tempo media, possiamo allora  
trovare la differenza di valore durante il tempo di osservazione.

$v_{medio} = \frac{-60 - 100}{100} = - \frac{8}{5} = -1.6$  

Si ha quindi che in media il valore diminuisce di $1.6$ al secondo, anche se  
questa informazione non ci dice molto in questo caso particolare data la natura del segnale.


## Q3 - Algebra dei sistemi  

![uda1_sistemi_lineari_e_segnali_fig3](https://user-images.githubusercontent.com/7195133/205507551-c906b4b7-ab95-4bc2-bea9-557f0616e4ea.jpg)  

Determinare la funzione di trasferimento del sistema.  
Determinare inoltre il valore di $X$, di $Z$ e di $W$
quando l’uscita del sistema è $150$.  

## Soluzione  

Applichiamo le note formule per il calcolo della funzione di trasferimento per  
collegamenti in serie e in parallelo.  

$F = (\frac{1}{5} \cdot 5) + (\frac{1}{5} \cdot 15) + 6 = \frac{1}{5} \cdot (5 + 15) + 6 = 4 + 6 = 10$  

Sapendo che $Y = X \cdot F$ allora $X = \frac{Y}{F}$ quindi  

$X = \frac{150}{10} = 15$  

Questo significa che quando $X = 15$ allora $W = 15 \cdot \frac{1}{5} \cdot 15 = 45$ mentre $Z = 15 \cdot 6  = 90$  


## Q4 - Algebra dei sistemi  

![uda1_sistemi_lineari_e_segnali_fig4](https://user-images.githubusercontent.com/7195133/205514956-f78dd2e8-7858-4922-b8a9-94599885453a.jpg)  

Determinare la funzione di trasferimento del sistema in figura.  

## Soluzione  

In sostanza si usa la formula per calcolare la funzione di trasferimento di un  
sistema collegato in retroazione negativa:  

$Y = \frac{F_1}{1 + F_1 \cdot F_2} \cdot X$  

Si deve solo semplificare il sistema in modo da ottenere le funzioni $F_1, F_2$ equivalenti.  

$F_1 = F_A \cdot F_B + F_A \cdot F_C= F_A \cdot (F_B + F_C)$  
$F_2 = F_D$  

$Y = F_1 \cdot V$  
$Z = F_2 \cdot Y$  
$V = X - Z$  

$Y = F_1 \cdot (X - Z) = F_1 \cdot X - F_1 \cdot Z$  
$Y = F_1 \cdot X - F_1 \cdot F_2 \cdot Y$  
$Y + F_1 \cdot F_2 \cdot Y = F_1 \cdot X$  
$Y \cdot (1 + F_1 \cdot F_2) = F_1 \cdot X$  
$Y = \frac{F_1}{1 + F_1 \cdot F_2} \cdot X$  
