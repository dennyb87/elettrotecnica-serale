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
la funzione di trasferimento e' $F = \frac{R_4}{R_4 + R_{eq}} = \frac{45}{60} = \frac{3}{4}$  
Allora possiamo risolvere trovando $V_1$ moltiplicando entrambe i termini  
dell'equazione per il reciproco di $F$ ovvero $\frac{1}{F} = \frac{R_4 + R_{eq}}{R_4}$. 

$V_1 = \frac{R_4 + R_{eq}}{R_4} \cdot V_2 = \frac{4}{3} \cdot V_2$  

Possiamo ora completare la tabella.  

| $V_1\ [V]$ | $V_2\ [V]$ |
| ---------- | ---------- |
| $0$        | $0$        |
| $100$      | $75$       |
| $-100$     | $-75$      |
| $20$       | $15$       |
| $30$       | $22.5$     |