# Seconda legge di Ohm  

$R = \rho \frac{l}{S}$  

La seconda legge di Ohm ci dice che la resistenza $R$ dipende dal rapporto che c'e' tra la lunghezza $l$ e la sezione $S$ del conduttore  
moltiplicato per un coefficiente di resistivita' $\rho$ (rho) che dipende dal tipo di materiale del conduttore stesso, e dalla temperatura.  
Il coefficiente di **resistivita' e' quindi la resistenza di un cavo di $1m$ di lunghezza e $1mm^2$ di sezione ad una determinata temperatura**.
Per esempio la resistivita' del rame a $20\degree C$ e' di $0.018 \cdot \frac{1m}{1mm^2} = 0.018 \Omega$  

Con sezione si intende l'area della sezione dell'anima in rame del cavo, ovvero $S = \pi \cdot r^2$

# Componenti attivi e passivi  

![componenti_attivi_passivi](https://user-images.githubusercontent.com/7195133/195986936-3c6034b4-7262-4f73-8b2d-723a0062323b.jpg)  

Si dicono **attivi** i componenti che forniscono energia e.g. il generatore $E$
Mentre si dicono **passivi** i componenti che assorbono energia e.g. il resistore $R$  

## Resistori in serie e in parallelo

Due resistori sono in **serie** quando hai capi hanno la stessa tensione, mentre sono in **parallelo** quando sono attraversate dalla stessa corrente.  


![resistori_in_serie_e_parallelo](https://user-images.githubusercontent.com/7195133/195977052-41a502ee-093f-4f7a-99c1-2cb5ba18965d.png)  

Calcolo **resistenza equivalente in parallelo** $R_{eq} = \frac{R_1 \cdot R_2}{R_1 + R_2}$  

Calcolo **resistenza equivalente in serie**  $R_{eq} = R_1 + R_2$  


In **parallelo** e' evidente che $I$ deve in qualche modo dividersi per passare un po' attraverso $R_1$ e un po' attraverso $R_2$.  
Si intuisce quindi che la corrente che entra nel nodo e' la somma delle due correnti che escono dal nodo $I = I_1 + I_2$ (vedi [Prima legge di Kirchoff](#prima-legge-di-kirchoff)).  
La tensione che c'e' su $R_1$ ed $R_2$ invece e' la stessa.


In **serie** invece, $R_1$ e $R_2$ sono attraversate dalla stessa corrente $I$, si intuisce quindi che la tensione deve cadere un po' su $R_1$ ed un po' su $R_2$, evidenziando come la somma della tensioni sia zero $V - V_1 - V_2 = 0$ in quanto il generatore produce una tensione $V$ mentre le resistenze fanno cadere rispettivamente $V_1$ e $V_2$, quindi e' anche vero che $V = V_1 + V_2$ (vedi [Seconda legge di Kirchoff](#seconda-legge-di-kirchoff)).  

E' *impoprtante* quindi notare che nell'esempio in **serie** $V_1 = V_b \cdot \frac{R_1}{R_{eq}}$ oppure $V_2 = V_b \cdot \frac{R_2}{R_{eq}}$



# Prima legge di Kirchoff 
#### Legge dei nodi
> La somma delle correnti entranti in un nodo è uguale alla somma delle correnti uscenti   

$I_1 = I_2 + I_3$

Un **nodo** e' un punto di confluenza di tre o piu' conduttori.


![kirchhoff_1](https://user-images.githubusercontent.com/7195133/195977379-bbc3de68-a649-4520-9e59-a086dc6534dd.jpg)  

# Seconda legge di Kirchoff  
#### Legge delle maglie  
> La somma algebrica delle differenze di potenziale che si trovano percorrendo una maglia e' uguale a zero.  

Una **maglia** e' un percorso chiuso all'interno di un circuito.  

![kirchhoff_2](https://user-images.githubusercontent.com/7195133/195985646-8b277b29-6bf0-44a7-9a6d-08240a51b0e8.jpg)  

Si noti come $V_s = V_{R_1} + V_{R_2} + V_{R_3}$ oppure $V_s - V_{R_1} - V_{R_2} - V_{R_3} = 0$

# Coulomb & Ampere

L'unita di misura della carica e' il **Coulomb** (dal fisico *Charles-Augustin de Coulomb*) e si indica con $C$, mentre il simbolo di carica e' $q$ o $Q$.  
Quando in un conduttore scorre un **Coulomb** di cariche al secondo si ha una corrente di un **Ampere** quindi $1A = \frac{1C}{1s}$

![coulomb_per_second](https://user-images.githubusercontent.com/7195133/217673362-dd269a26-153d-4af3-9fad-372fec198933.jpg)


# Fusibile  

![fusibile](https://user-images.githubusercontent.com/7195133/197292192-fcb41db8-830b-4991-b14c-a9a04cdbd4cc.gif)

Un fusibile è un dispositivo elettrico in grado di proteggere un circuito dalle sovracorrenti.  
Contiente un filamento di tungsteno che si fonde, quindi interrompendo il circuito, una volta raggiunta una soglia  
di calore provocato dalla corrente.  



