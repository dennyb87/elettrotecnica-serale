# Verifica delle leggi di Kirchhoff e conservazione dell'energia  

Si prenda in considerazione il seguente circuito e scriviamo le grandezze note.  
$E = 38V$  
$R_1 = 2 \Omega$  
$R_2 = 1\Omega$  
$R_3 = 3 \Omega$  
$R_4 = 5\Omega$  

![circuito_verifica_leggi](https://user-images.githubusercontent.com/7195133/202846278-7e68d9fe-953f-4a6d-8034-6ae564f37fef.jpg)  

Possiamo allora trovare la resistenza equivalente in parallelo:  

$R_s = R_2 + R_3 = 4\Omega$  
$R_p = \frac{R_s \cdot R_4}{R_s + R_4} = 2.\overline{2}\Omega$  

Successivamente si puo' trovare $I_1$ che e' uguale alla tensione del generatore  
sulla resistenza totale.  

$R_{tot} = R_1 + R_p = 4.\overline{2}\Omega$  
$I_1 = \frac{E}{R_{tot}} = \frac{38}{4.\overline{2}}= 9A$  

Se la caduta di potenziale $V_{AB} = I_1 \cdot R_1 = 18V$ allora $V_{BF} = V_{AF} - V_{AB} = 38 - 18 = 20V$.  
Sapendo che in parallelo i componenti sono soggetti alla stessa tensione allora  

$I_2 = \frac{V_{BF}}{R_s} = \frac{20}{4} = 5A$  
$I_4 = \frac{V_{BF}}{R_4} = \frac{20}{5} = 4A$  

Adesso possiamo trovare le cadute di potenziale mancanti.  

$V_{BC} = I_2 \cdot R_2 = 5 \cdot 1 = 5V$  
$V_{CF} = I_2 \cdot R_3 = 5 \cdot 3 = 15V$  

Mettiamo un po' di ordine.  

| tensioni | [V]  |
| -------- | ---- |
| $V_{AF}$ | $38$ |
| $V_{AB}$ | $18$ |
| $V_{BC}$ | $5$  |
| $V_{CF}$ | $15$ |
| $V_{BF}$ | $20$ |


# IPK - Verifica del primo principio di Kirchhoff  

$I_1 = I_2 + I_4$  
$9 = 5 + 4$  

Verificato $\checkmark$  

# IIPK - Verifica del secondo principio di Kirchhoff  

Maglia $A \rightarrow B \rightarrow C \rightarrow F \rightarrow A$

$V_{AF} = V_{AB} + V_{BC} + V_{CF}$  
$38 = 18 + 5 + 15$  

Verificato $\checkmark$  

Maglia $B \rightarrow F \rightarrow C \rightarrow B$

$V_{BF} = V_{BC} + V_{CF}$  
$20 = 5 + 15$  

Verificato $\checkmark$  

# Verifica della legge di conservazione dell'energia  

| potenze | calcolo      | [W]   |
| ------- | ------------ | ----- |
| $P_E$   | $38 \cdot 9$ | $342$ |
| $P_1$   | $18 \cdot 9$ | $162$ |
| $P_2$   | $5 \cdot 5$  | $25$  |
| $P_3$   | $15 \cdot 5$ | $75$  |
| $P_4$   | $20 \cdot 4$ | $80$  |

$P_E = P_1 + P_2 + P_3 + P_4$  
$342 = 162 + 25 + 75 + 80$  

Verificato $\checkmark$  