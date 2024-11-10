# Dimensionamento di un impianto  

![dim_impianto_01](https://github.com/user-attachments/assets/92da6f22-7ef2-4c4a-ad4b-9d77fe345944)  

Si vuole dimensionare l'impianto di un officina meccanica con le seguenti caratteristiche:  

$S = 80\ \frac{VA}{m^2}$  
$A = 500\ m^2$  
$\ell = 40\ m$  
$\cos \varphi = 0.9$  

Cavi **unipolari** in **EPR**

### Potenza convenzionale  

$P_c = S \cdot A \cdot \cos \varphi = 80 \cdot 500 \cdot 0.9 = 36\ kW$  

Essendo $P_c > 6\ kW$ si utilizza un sistema trifase.  

### Corrente di impiego  

$I_b = \dfrac{P_c}{\sqrt{3}\cdot V\cdot\cos \varphi} = \dfrac{3600}{\sqrt{3}\cdot 400\cdot 0.9} \simeq 58\ A$  

### Condizioni di protezione sovraccarico  

Per la protezione da sovraccarico si utilizzano interruttori magnetotermici con una corrente nominale d'intervento $I_n$ compresa tra la corrente d'impiego $I_b$ e la portata della linea $I_z$  

$I_b \le I_n \le I_z$  

Questo permette all'interruttore di ignorare la normale corrente d'esercizio, ma allo stesso tempo evitare di raggiungere correnti che danneggerebbero la linea.  

### Caduta di tensione  

Per scegliere l'interruttore di protezione si deve prima trovare la portata $I_z$ della linea. Si ipotizza che la caduta di tensione ammissibile sia:  

```math
\Delta V \% \le 1\ \%
```

$u = \dfrac{\Delta V \cdot 1000}{I_b \cdot \ell} = \dfrac{4 \cdot 1000}{58 \cdot 40} \simeq 1.72\ \frac{mV}{am}$  

Dalle apposite tabelle per un sistema trifase con cavi unipolari si ricava una sezione di $25\ mm^2$ da cui, considerando i coefficienti unitari, si ottiene una portata di $100\ A$  

$58 \le I_n \le 100$  

Per soddisfare la condizione si sceglie quindi un interruttore da $I_n = 63\ A$ con un potere di interruzione da $15\ kA$  

### Protezione da contatti indiretti  

La protezione si ottiene utilizzando un interruttore differenziale con un appropriato impianto di terra in modo da rispettare la tensione di contatto limite $U_L$ che in ambienti ordinari e' $50\ V$  

$R_E \cdot I_{dn} \le U_L$  

Ipotizzando una resistivita' del terreno di $\rho = 300\ \Omega m$ utilizzando le apposite tabelle si scelgono due picchetti in parallelo di diametro $\varnothing = 18\ mm$ e lunghezza $\ell = 3\ m$ in acciaio zincato a caldo di resistenza $R_{Ep} = 95.6\ \Omega$  

Assicursandosi di distanziare i picchetti di $3$ volte la loro lunghezza e' possibile utilizzare la seguente formula per stimare la resistenza di dispersione totale, dove $N$ e' il numero di dispersori.  

$R_E = \dfrac{R_{Ep}}{N} = \dfrac{95.6}{2} = 47.8\ \Omega$  

Dalle tabelle secgliamo il differenziale con la corrente di intervento maggiore $I_{dn} = 1\ AS$ dove $S$ sta' per selettivo, per soddisfare la condizione di protezione.  

$47.8 \cdot 1 \le 50$  

