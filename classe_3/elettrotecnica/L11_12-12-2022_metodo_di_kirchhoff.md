# Il metodo di Kirchhoff per risolvere i circuiti elettrici  

Risolvere un circuito elettrico significa trovare i valori delle grandezze elettriche  
in ogni parte del circuito, quindi tutte le correnti, tensioni, e resistenze.  
Il metodo di Kirchhoff consiste nell'impostare un sistema di equazioni, in particolare   
le equazioni ai nodi, e alle maglie.  
Le equazioni saranno pari al numero di grandezze incognite del cicuito, in questo caso  
pari al numero di correnti, e quindi al numero di rami.  

Andiamo allora a risolvere il circuito seguente.  

![metodo_di_kirchhoff_01](https://user-images.githubusercontent.com/7195133/208296544-6e0b21d2-e5b2-4df6-b885-07b1f49262cd.jpg)



## Equazioni ai nodi  

Il sistema deve contenere le equazioni ai nodi e alle maglie.  
Si utilizza quindi il primo principio di Kirchhoff per scrivere le equazioni ai nodi.  
Il numero di equazioni sara' pari al numero di nodi meno uno, ovvero $n - 1$, in quanto  
e' dimostrato che l'ultimo nodo non aggiunge informazione, e puo' essere quindi ignorato.  
Basta notare che l'equazione al nodo $D$ e' in effeti uguale all'equazione del nodo $B$.  


| nodo | equazione         |
| ---- | ----------------- |
| $B$  | $I_1 + I_2 = I_3$ |
| $D$  | $I_3 = I_1 + I_2$ |

Dato che sono uguali possiamo sceglierne una, diciamo l'equazione al nodo $B$.  

$I_1 + I_2 = I_3$  

## Equazioni alle maglie  

Poniamo per semplicita'  

$V_{AB} = V_1$
$V_{CB} = V_2$
$V_{BD} = V_3$


Per le equazioni alle maglie si usa ovviamente il secondo principio di Kirchhoff  
per ogni maglia, ovvero:  

$V_1 + V_2 - E_1 = 0$  
$E_2 - V_2 - V_3 = 0$


# Sistema di equazioni  

Il sistema ci permette di trovare le correnti incognite, per adesso utilizzeremo  
il metodo della sostituzione, ma ce ne sono ovviamente altri.  

$$
\begin{cases}
  \begin{aligned}
    I_1 + I_2 - I_3 &= 0 \\
    V_1 + V_3 - E_1 &= 0 \\
    E_2 - V_2 - V_3 &= 0 \\
  \end{aligned}
\end{cases}
$$

Sostituiamo le tensioni con le formule equivalenti servendoci della legge di Ohm

$$
\begin{cases}
  \begin{aligned}
    I_1 + I_2 - I_3 &= 0 \\
    R_1 I_1 + R_3 I_3 - E_1 &= 0 \\
    E_2 - R_2 I_2 - R_3 I_3 &= 0 \\
  \end{aligned}
\end{cases}
$$


Impostato il sistema possiamo sostituire una delle correnti ad esempio $I_3$ alla  
seconda equazione con l'equivalente $I_3 = I_1+ I_2$

$R_1 I_1 + R_3 I_3 - E_1 = 0$  
$10I_1 + 30I_3 - 100 = 0$  
$10I_1 + 30 \cdot (I_1 + I_2) - 100 = 0$  
$40I_1 + 30I_2 - 100 = 0$


Riscriviamo allora sistema


$$
\begin{cases}
  \begin{aligned}
    I_3 &= I_1 + I_2 \\
    40I_1 + 30I_2 - 100 &= 0 \\
    E_2 - R_2 I_2 - R_3 I_3 &= 0 \\
  \end{aligned}
\end{cases}
$$


Procediamo ora con la terza equazione  

$50 - R_2 I_2 - R_3 I_3 = 0$  
$50 - 20 I_2 - 30 \cdot (I_1 + I_2) = 0$  
$50 - 20 I_2 - 30I_1 - 30I_2 = 0$  
$50 - 50I_2 - 30I_1 = 0$  


Riscriviamo allora sistema

$$
\begin{cases}
  \begin{aligned}
    I_3 &= I_1 + I_2 \\
    40I_1 + 30I_2 - 100 &= 0 \\
    50 - 50I_2 - 30I_1 &= 0 \\
  \end{aligned}
\end{cases}
$$

Isoliamo $I_2$  

$50 - 50I_2 - 30I_1 = 0$  
$-50I_2  = 30I_1 - 50$  
$50I_2 = - 30I_1 + 50$  
$I_2 = \dfrac{50 - 30I_1}{50}$  


Sostituiamo ora $I_2$ alla seconda equazione per trovare $I_1$

$40I_1 + 30I_2 - 100 = 0$  
$40I_1 + 30 \cdot \dfrac{50 - 30I_1}{50} - 100 = 0$  
$40I_1 + 30 \cdot (1 - \frac{30}{50}I_1) - 100 = 0$  
$40I_1 + 30 - 18I_1 - 100 = 0$  
$22I_1 - 70 = 0$  
$I_1 = \dfrac{70}{22} = 3.18A$  

Da finire ...
