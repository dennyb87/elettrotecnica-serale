# Risoluzione di un circuito con Kirchhoff  

![risoluzione_circuito_con_kirchhoff](https://user-images.githubusercontent.com/7195133/204092042-efe83286-c0c0-44c3-aaca-f17fc6e5a2d7.jpg)  

Ci vengono date le resistenze, la tensione fornita dal generatore, e tre correnti.  

$I_0 = 6.744A$  
$I_1 = 3.548A$  
$I_5 = 0.645A$  

Possiamo allora iniziare trovando le correnti non ancora note applicando la prima  
legge di Kirchhoff $I_1 + I_3 = I_0$ ovvero $I_3 = I_0 - I_1 = 6.744 - 3.548 = 3.196A$ e cosi via...

$I_2 = I_1 - I_5 = 3.548 - 0.645 = 2.903A$  
$I_4 = I_5 + I_3 = 0.645 + 3.196 = 3.841A$  

Abbiamo verificato la prima legge Kirchhoff sui nodi $A, B, D$, controlliamo quindi anche $C$  
### IPK nodo C  
$I_0 = I_2 + I_4 = 2.903 + 3.841 = 6.744A \ \ verificato\ \checkmark$  

Adesso non resta che trovare le cadute di potenziale con la legge di Ohm.  

|       | $Ohm's\ law$    | $[V]$    |
| ----- | --------------- | -------- |
| $V_1$ | $I_1 \cdot R_1$ | $70.96$  |
| $V_2$ | $I_2 \cdot R_2$ | $29.03$  |
| $V_3$ | $I_3 \cdot R_3$ | $79.9$   |
| $V_4$ | $I_4 \cdot R_4$ | $19.205$ |
| $V_5$ | $I_5 \cdot R_5$ | $9.675$  |


Verifichiamo ora la seconda legge di Kirchhoff per $V_5$.  

*La tensione tra due punti e' uguale alla somma algebrica delle tensioni  
incontrate in uno qualsiasi dei percorsi che connettono tra loro i due punti*  

Essenzialmente ci dice che la tensione tra $B$ e $D$ e' uguale alla somma  
algebrica delle tensioni incontrate per andare da $B$ a $D$ in senso antiorario  
senza passare da $R_5$ ovvero:
 
$V_{BD} = V_{BC} + V_{CD}$  
$V_{BD} = V_2 - V_4 = 9.825V$    

Oppure prendendo in considerazione i punti $A, B, D$  

$V_{BD} = V_{BA} + V_{AD} = - V_1 + V_3 = 8.94V$  

Purtroppo le approssimazioni delle correnti non ci hanno permesso di ottenere un  
risultato molto preciso, c'e' quindi una differenza di circa $1V$ per cui:  

$V_{BC} + V_{CD} \simeq V_{BA} + V_{AD}$  
$9.825V \simeq 8.94V$  

Riteniamo comunque la legge verificata $\checkmark$