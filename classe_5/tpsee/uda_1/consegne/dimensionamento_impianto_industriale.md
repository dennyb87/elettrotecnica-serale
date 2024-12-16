# Dimensionamento impianto industriale  

![componenti_inpianto_industriale](https://github.com/user-attachments/assets/4146d858-064e-4321-a85c-ac7bb19a9b9a)  

Si vuole dimensionare l'impianto elettrico alimentato in **bassa tensione** di un capannone industriale adibito al taglio e alla foratura di lamiere metalliche.  

I pannelli prese **CEE** interbloccate sono costituiti da:  

* 1 presa trifase, **3P+T**, $400\ V,\ 16\ A$
* 3 prese monofasi, **2P+T**, $230\ V,\ 16\ A$

Per le prese si ipotizza un fattore di potenza di $0.9$.  

## Potenza convenzionale  

Procediamo a calcolare le potenze convenzionali dei rispettivi quadri ipotizzando un quadro generale **QE1**  che controlla quattro quadri **QE2-5** e il **reparto di lavorazione**.  

### QE2 - Ufficio e cortile  

Si ipotizza che le utenze del cortile verranno comandate dall'ufficio.  

| Utenze       | $P_n[\text{kW}]$ | $K_u$ | $K_c$ | $P_c[\text{kW}]$ |
| ------------ | ---------------- | ----- | ----- | ---------------- |
| luci interne | 0.3              | 1     | 1     | 0.3              |
| luci esterne | 0.2              | 1     | 0.4   | 0.08             |
| prese        | 12.8             | 1     | 0.15  | 1.92             |
| utenze varie | 0.7              | 1     | 0.4   | 0.28             |
|              |                  |       |       | 2.58             |

### QE3 - Magazzino  

| Utenze | $P_n[\text{kW}]$ | $K_u$ | $K_c$ | $P_c[\text{kW}]$ |
| ------ | ---------------- | ----- | ----- | ---------------- |
| luci   | 0.72             | 1     | 1     | 0.72             |
| prese  | 39.9             | 1     | 0.15  | 6                |
|        |                  |       |       | 6.72             |

### QE4 - Spogliatoio  

| Utenze      | $P_n[\text{kW}]$ | $K_u$ | $K_c$ | $P_c[\text{kW}]$ |
| ----------- | ---------------- | ----- | ----- | ---------------- |
| luci        | 0.216            | 1     | 1     | 0.216            |
| prese       | 10.35            | 1     | 0.15  | 1.55             |
| scaldabagno | 1.5              | 1     | 1     | 1.5              |
|             |                  |       |       | 3.27             |


### QE5 - Officina  

| Utenze | $P_n[\text{kW}]$ | $K_u$ | $K_c$ | $P_c[\text{kW}]$ |
| ------ | ---------------- | ----- | ----- | ---------------- |
| luci   | 0.3              | 1     | 1     | 0.3              |
| prese  | 100              | 1     | 0.15  | 15               |
|        |                  |       |       | 15.3             |

### QE1 - Generale  

| Utenze          | $P_n[\text{kW}]$ | $K_u$ | $K_c$ | $P_c[\text{kW}]$ |
| --------------- | ---------------- | ----- | ----- | ---------------- |
| QE2,QE3,QE4,QE5 | 27.87            | 1     | 0.7   | 19.5             |
| stazione 1      | 35               | 0.8   | 0.7   | 19.6             |
| stazione 2      | 35               | 0.8   | 0.7   | 19.6             |
| stazione 3      | 35               | 0.8   | 0.7   | 19.6             |
| compressore     | 12               | 0.8   | 0.8   | 7.68             |
| illuminazione   | 4.8              | 1     | 1     | 4.8              |
| prese           | 139.67           | 1     | 0.15  | 20.95            |
| GAC             | 0.8              | 1     | 1     | 0.8              |
|                 |                  |       |       | 112.53           |


Applicando un ulteriore fattore di contemporaneita' ed utilizzo otteneniamo una potenza convenzionale complessiva di...  

$P_c = 112.53 \cdot 0.7 = 78.77 \simeq 80\ kW$  

## Dimensionamento linea QE1  

Andiamo a calcolare la corrente d'impiego $I_b$ della linea tra il punto di consegna **PDC** e il quadro generale.  

$I_b = \dfrac{P_c}{\sqrt{3}\cdot 400} = \dfrac{80\ 000}{\sqrt{3}\cdot 400}\simeq 115\ A$  

Si ipotizza una caduta di potenziale massima di 1% ovvero $\Delta V = 4\ V$ su una linea di $30\ m$  

$$
u = \dfrac{\Delta V \cdot 1000}{I_b\cdot\ell} = \dfrac{4\cdot 1000}{115\cdot 30}\simeq 1.16\ \tiny{\frac{mV}{Am}}
$$

Dalla tabella a pagina **X-77** del manuale con trifase $\cos\varphi = 0.9$ ricaviamo una sezione di $35\ mm^2$. Ipotizzando *cavi unipolari* in **EPR** posati in tubi interrati tra loro a contatto, troviamo a pagina **X-68** proprio una $I_0 = 133\ A$ che soddisfa la condizione $I_b \le I_n \le I_z$ considerando condizioni di posa e temperatura ambiente tali da poter utilizzare coefficienti unitari. Si ha llora che...  

$I_z = I_0 = 133\ A$  

$115 \le I_n \le 133\ A$  

Scegliamo quindi un **magnetotermico modulare** con $I_n = 125\ A$ ed essendo una fornitura trifase per una $P_c > 33\ kW$ e una $I_b = 115\ A$ lo scegliamo con un potere di interruzione di $15\ kA$ consultando pagina **XXIV-14**.  

### Dimensionamento linea QE5  

Applichiamo un ulteriore fattore di contemporaneita' ed utilizzo per una potenza convenzionale di...  

$P_c = 15.3 \cdot 0.9 = 13.77\ kW$  

Si ha allora che la corrente di impiego sulla linea per il quadro **QE5** e' di:  

$I_b = \dfrac{P_c}{\sqrt{3}\cdot 400} = \dfrac{13\ 770}{\sqrt{3}\cdot 400} \simeq 19.88\ A$  

Si ipotizza una caduta di potenziale massima di 2.5% ovvero $\Delta V = 10\ V$ su una linea di circa $30\ m$  

$$
u = \dfrac{\Delta V \cdot 1000}{I_b\cdot\ell} = \dfrac{10\cdot 1000}{19.88\cdot 30}\simeq 16.76\ \frac{mV}{Am}
$$

Dalla tabella a pagina **X-77** del manuale con trifase $\cos\varphi = 0.9$ ricaviamo una sezione di $2.5\ mm^2$.  

Ipotizzando *cavi unipolari* in **EPR** posati in aria su passerelle perforate (posa 13), troviamo a pagina **X-60** una $I_0 = 33\ A$. Nella stessa passerella sara' presente il circuito dello spogliatoio (**QE4**) per cui dalla tabella a pagina X-64 scegliamo un $K_1 = 0.88$ mentre la temperatura ambiente ci permette di utilizzare un coefficitente unitario.  

$I_z = I_0\cdot K_1\cdot K_2= 33\cdot 0.88\cdot 1 = 29.4\ A$  

$19.88 \le I_n \le 29.04\ A$  

Per soddisfare la condizione di protezione da sovracorrenti segliamo a pagina **X-113** un **magnetotermico modulare** con $I_n = 25\ A$  

$19.88 \le 25 \le 29.04\ A$  


## QE4, QE3, QE2  

I quadri restanti hanno potenze minori e a maggior ragione e' possibile installare cavi della stessa sezione garantendo cadute di tensioni minori, o coprire maggiori distanze a parita' di caduta di tensione. Pertanto prevediamo di installare **magnetotermici modulari** da $I_n = 25\ A$ anche per questi quadri. Ad esempio per il magazzino **QE3** con $P_c = 6.72\ kW$ si avra' una corrente di impiego...  

$I_b = \dfrac{P_c}{\sqrt{3}\cdot 400} = \dfrac{6\ 720}{\sqrt{3}\cdot 400} \simeq 9.7\ A$  

Ipotizzando la stessa caduta di potenziale massima di 2.5% ovvero $\Delta V = 10\ V$ su una linea di circa $50\ m$ si avrebbe...    

$$
u = \dfrac{\Delta V \cdot 1000}{I_b\cdot\ell} = \dfrac{10\cdot 1000}{9.7\cdot 50}\simeq 20.62\ \tiny{\frac{mV}{Am}}
$$

Dalla tabella a pagina **X-77** del manuale con trifase (ma soddisfatta anche nel monofase) $\cos\varphi = 0.9$ ricaviamo una sezione di $2.5\ mm^2$ che sappiamo essere in accordo con le considerazioni di posa e quindi con la portata.  

$I_b \le I_n \le I_z = 9.7 \le 25 \le 29.04\ A$  

## Protezione da contatti indiretti  

La protezione si ottiene utilizzando interruttori differenziali insieme ad un appropriato impianto di terra in modo da rispettare la tensione di contatto limite $U_L$ che in ambienti ordinari e' $50\ V$  

$R_E \cdot I_{dn} \le U_L$  

Ipotizzando una resistivita' del terreno di $\rho = 300\ \Omega m$ dalle tabelle a pagina **X-172** del manuale si scelgono due picchetti in parallelo di diametro $\varnothing = 18\ mm$ e lunghezza $\ell = 3\ m$ in acciaio zincato a caldo di resistenza $R_{Ep} = 95.6\ \Omega$  

Assicursandosi di distanziare i picchetti di $6$ volte la loro lunghezza e' possibile utilizzare la seguente formula per stimare la resistenza di dispersione totale, dove $N$ e' il numero di dispersori.  

$R_E = \dfrac{R_{Ep}}{N} = \dfrac{95.6}{2} = 47.8\ \Omega$  

Consultando il manuale a pagina **X-176** scegliamo per il quadro generale **QE1** il differenziale con la corrente di intervento maggiore $I_{dn} = 1\ A$ di tipo **S** (selettivo) per soddisfare la condizione di protezione.  

$47.8 \cdot 1 \le 50\ V$  

Per gli altri quadri scegliamo dei differenziali con $I_n = 30\ mA$  

## Installazione dei quadri  

![pianta](https://github.com/user-attachments/assets/efe3d4b7-6fba-48d2-bf38-53631b93bea4)  

Si ipotizza un'installazione come in figura, dove il quadro generale **QE1** viene posizionato all'ingresso ma allo stesso tempo vicino al quadro dai maggiori consumi, ovvero **QE5**, in modo da minimizzare la distanza della linea e di conseguenza la caduta di tensione.  

Per gli altri quadri si prevedono correnti minori per cui avremo piu' flessibilita' sulle distanze.  
