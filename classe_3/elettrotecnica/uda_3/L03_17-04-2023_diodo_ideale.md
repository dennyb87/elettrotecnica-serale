# Il diodo ideale  

Sappiamo che il diodo e' un componente elettronico, ovvero un semiconduttore, di piccola potenza, orientato al controllo ed elaborazione dell'informazione. Il diodo ideale puo' essere in due stati:

* **DIODO ON** - *in conduzione*
* **DIODO OFF** - *interdetto*

![ideal_diode](https://user-images.githubusercontent.com/7195133/233193230-eba2bec1-60ad-4861-b4bb-c9356fdf756d.jpg)

In polarizzazione diretta o *forward bias* vediamo allora il diodo *in conduzione*, ovvero l'equivalente di un corto circuito. E' importante notare che quando il diodo e' in conduzione, la caduta di potenziale su di esso e' zero, come si puo' notare nella curva caratteristica.  

Mentre in polarizzazione inversa o *reverse bias* il diodo e' interdetto, e il circuito si presenta come *aperto*, dove in questo caso la tensione e' negativa.  

Possiamo allora concludere che il diodo ideale e' un componente che non dissipa potenza, anche se sappiamo benissmo che in pratica questo non e' possibile.  

## Diodo ideale in un circuito  

Analizziamo ora il seguente circuito nel caso di un diodo $D$ in polarizzazione inversa, ovvero l'equivalente di un circuito aperto.  

![diode_off](https://user-images.githubusercontent.com/7195133/233206825-f806284d-5e23-43e3-9780-1c2d2157ea53.jpg)  

In questo caso allora la corrente sul diodo e' zero, percio' possiamo trovare $R_{tot}$ sommando le resistenze ed infine trovare la corrente $I$ nel circuito.  

$I_D = 0$  

$R_{tot} = R_1 + R_2 = 4000 + 6000 = 10\ k\Omega$  

$I = I_1 = I_2 = \dfrac{E}{R_{tot}} = \dfrac{20}{10000} = 2\ mA$  

![diode_on](https://user-images.githubusercontent.com/7195133/233210963-c4fa146f-869c-4cff-86ce-9ce9acce8a91.jpg)  

In questo caso invece $D$ causa un corto circuito, di fatto rendendo $R_2$ trascurabile in quanto non causa nessuna caduta di potenziale dato che la resistenza sul diodo e' $R_D = 0\ \Omega$ questo e' dimostrabile applicando il partitore di corrente.  

$I_2 = \dfrac{R_D}{R_2 + R_D} \cdot I = \dfrac{0}{R_2} \cdot I= 0$  

$V_2 = V_{BC} = R_2 \cdot I_2 = 6000 \cdot 0 = 0\ V$  

Si ha allora zero caduta di potenziale su $R_2$ mentre la resistenza totale e' $R_{tot} = R_1$ quindi...

$I = I_1 = \dfrac{E}{R_1} = \dfrac{20}{4000} = 5\ mA$  
