# UDA 1 – CORRENTE ELETTRICA CONTINUA

## ESERCIZIO N. 1  

![elt_uda1_corrente_continua_fig1](https://user-images.githubusercontent.com/7195133/204739070-0d2d930c-5a30-4835-91a2-7dc579be7182.jpg)  

Sapendo che $R = 10\Omega$ calcolare la resistenza totale vista dai morsetti $A, B$  
nel circuito mostrato in figura.  

## Soluzione  

Per trovare $R_{tot}$ ci basta semplificare il circuito.  
Per farlo possiamo utilizzare le formule per il calcolo delle resistenze in serie  
e parallello. La prima semplificazione possibile e' quella dell'ultima maglia a  
destra, percio' partiamo da li'.

$R_{P1} = \frac{R_1 \cdot R_2}{R_1 + R_2}$ ma $R = R_1 = R_2$ allora...  
$R_{P1} = \frac{R^2}{2R} = \frac{R}{2}$  
$R_{S1} = R + R_{P1} = R +\frac{R}{2} = \frac{3R}{2}$    
$R_{P2} = \frac{R \cdot R_{S1}}{R + R_{S1}} = \frac{R \cdot \frac{3R}{2}}{R + \frac{3R}{2}} = \frac{3R^2}{2} \cdot \frac{2}{5R} = \frac{3R}{5}$  
$R_{tot} = R + R_{P2} = R + \frac{3R}{5} = \frac{8R}{5} = \frac{8 \cdot 10}{5} = 16\Omega$


## ESERCIZIO N. 2  

![elt_uda1_corrente_continua_fig2](https://user-images.githubusercontent.com/7195133/204798498-ee5d28d6-4b54-415a-b9a5-b42b496ae96f.jpg)  

Nel circuito mostrato in figura calcolare:  

1. la resistenza totale $R_{tot}$ del circuito
2. la corrente $I_0$ erogata dal generatore di tensione $E$
3. le cadute di tensione $V_{AC}, V_{CB}$
4. le correnti $I_1, I_2$
5. la potenza $P_E$ erogata dal generatore $E$
6. le potenze $P_R, P_{R1}, P_{R2}$ assorbite da ciascuna delle resistenze  
   presenti nel circuito. Verificare quindi i risultati ottenuti applicando:
   1. la $I$ legge di Kirchhoff al nodo $C$
   2. la $II$ legge di Kirchhoff alla maglia costituita dal generatore $E$  
      e dalle resistenze $R, R_1$
   3. il principio di conservazione dell'energia.


## Soluzione  

Per trovare la resistenza totale bisgna semplificare il circuito utilizzando le  
formule per il calcolo delle resistenze in serie e parallello.  

$R_p = \frac{R_1 \cdot R_2}{R_1 + R_2} = \frac{10 \cdot 30}{10 + 30} = 7.5\Omega$  
$R_{tot} = R + R_p = 2.5 + 7.5 = 10\Omega$  

La corrente puo' ora essere trovata con la legge di Ohm $I_0 = \frac{E}{R_{tot}} = \frac{200}{10} = 20A$  
cosi' come la caduta di tensione $V_{AC} = I_0 \cdot R = 20 \cdot 2.5 = 50V$  
Mentre la caduta di tensione $V_{CB}$ puo' ora essere derivata semplicemente con:  
$V_{CB} = E - V_{AC} = 200 - 50 = 150V$  
Ma controlliamo comunque che sia in accordo con la legge di Ohm:

$V_{CB} = I_0 \cdot R_p = 20 \cdot 7.5 = 150V$  

Le correnti $I_1, I_2$ sempre grazie alla legge di Ohm sono:

$I_1 = \frac{V_{CB}}{R_1} = \frac{150}{10} = 15A$  
$I_2 = \frac{V_{CB}}{R_2} = \frac{150}{30} = 5A$  

La potenza erogata dal generatore e' $P_E = V \cdot I_0 = 200 \cdot 20 = 4000W$  
Mentre le potenze assorbite dalle singole resistenze sono:  

$P_R = V_{AC} \cdot I_0 = 50 \cdot 20 = 1000W$  
$P_{R1} = V_{CB} \cdot I_1 = 150 \cdot 15 = 2250W$  
$P_{R2} = V_{CB} \cdot I_2 = 150 \cdot 5 = 750W$  

## IPK  
Nodo $C$
  $I_0 = I_1 + I_2 = 15 + 5 = 20A \ verificato\ \checkmark$  

## IIPK
Maglia $A \rightarrow C \rightarrow B \rightarrow A$  
$V_{AC} + V_{CB} + V_{BA} = 0$  
$50 + 150 - 200 = 0\ verficato\ \checkmark$


## Principio di conservazione dell'energia  
$P_E = P_R + P_{R1} + P_{R2}$  
$4000 = 1000 + 2250 + 750\ verfificato\ \checkmark$


## ESERCIZIO N. 3  

Si consideri una lampada che assorbe la potenza $P_L = 100W$ quando la tensione  
applicata è $V_L = 230V$. Calcolare la resistenza equivalente $R_L$ della lampada.  

## Soluzione  
Si procede trovando la corrente $I_L = \frac{P_L}{V_L} = \frac{1000}{230} \simeq 4.35A$  
Di conseguenza la resistenza della lampada e' $\frac{V_L}{I_L} = \frac{230}{4.35} \simeq 52.87\Omega$


## ESERCIZIO N. 4  

![elt_uda1_corrente_continua_fig3](https://user-images.githubusercontent.com/7195133/204860768-c12eab47-8a5b-49df-bf98-0c2dd1a44941.jpg)  

Per il circuito mostrato in figura calcolare:
1. la resistenza totale $R_{tot}$
2. la corrente $I_0$
3. la corrente $I_2$ e la corrente $I_4$   

## Soluzione  

Per trovare $R_{tot}$ bisogna ancora una volta semplificare il circuito utilizzando  
le note formule per il calcolo di resistenze in serie e parallelo.  

$R_{s1} = R_5 + R_6 = 30 + 30 = 60\Omega$  
$R_{p1} = \frac{R_4 \cdot R_{s1}}{R_4 + R_{s1}} = \frac{20 \cdot 60}{20 + 60} = \frac{1200}{80} = 15\Omega$  
$R_{s2} = R_3 + R_{p1} = 20 + 15 = 35\Omega$  
$R_{p2} = \frac{R_2 \cdot R_{s2}}{R_2 + R_{s2}} = \frac{10 \cdot 35}{10 + 35} = \frac{350}{45} = 7.78\Omega$  
$R_{tot} = R_1 + R_{p2} = 10 + 7.78 = 17.78\Omega$  

$I_0 = \frac{E}{R_{tot}} = \frac{180}{17.78} = 10.12A$  

Adesso applichiamo la formula del partitore di corrente.  

$I_2 = \frac{R_{s2}}{R_2 + R_{s2}} \cdot I_0 = \frac{35}{45} \cdot 10.12 = 7.87A$  
$I_3 = \frac{R_2}{R_2 + R_{s2}} \cdot I_0 = \frac{10}{45} \cdot 10.12 = 2.25A$  
$I_4 = \frac{R_{s1}}{R_4 + R_{s1}} \cdot I_3 = \frac{60}{80} \cdot 2.25 = 1.69A$  
$I_5 = \frac{R_4}{R_4 + R_{s1}} \cdot I_3 = \frac{20}{80} \cdot 2.25 = 0.56A$


### IPK  
$I_3 = I_4 + I_5 = 1.69 + 0.56 = 2.25A\ verificato\ \checkmark$
$I_0 = I_2 + I_3 = 7.87 + 2.25 = 10.12A\ verificato\ \checkmark$

## ESERCIZIO N. 5  

![elt_uda1_corrente_continua_fig4](https://user-images.githubusercontent.com/7195133/205460813-487cfb99-02a2-464c-934e-4b6e8cc5bd40.jpg)  

E’ assegnato il circuito elettrico mostrato in figura.  

Si chiede di:

1. indicare il numero di componenti, di punti di connessione, di nodi, di rami
2. determinare la corrente nei vari rami del circuito
3. calcolare la potenza erogata dal generatore e la potenza assorbita  
   da ciascun resistore
4. verificare il principio di conservazione dell’energia  

## Soluzione  

Il circuito ha 5 componenti, 1 generatore (attivo), e 4 resistenze (passive).  
Ci sono 4 punti di connessione, di cui solo 2 sono nodi $A, C$, mentre i rami  
per definizione sono invece 3.  

Per trovare la corrente ci serve prima di tutto $R_{tot}$  

$R_s = R_3 + R_4 = 4 + 4 = 8\Omega$  
$R_p = \frac{R_2 \cdot R_s}{R_2 + R_s} = \frac{6 \cdot 8}{6 + 8} = \frac{48}{14} = 3.43\Omega$  
$R_{tot} = R_1 + R_p = 2 + 3.43 = 5.43\Omega$  

Adesso possiamo applicare la legge di Ohm per trovare le correnti e tensioni:  

$I_1 = \frac{E}{R_{tot}} = \frac{40}{5.43} = 7.37A$  
$V_1 = I_1 \cdot R_1 = 7.37 \cdot 2 = 14.74V$  
$V_{AC} = V_{AD} + V_{DC} = E - V_1 = 40 - 14.74 = 25.26V$  
$I_2 = \frac{V_{AC}}{R_2} = \frac{V_2}{R_2} = \frac{25.26}{6} = 4.21A$  

In questo caso ci serviamo di un caso particolare del partitore di tensione visto che  $R_3 = R_4 = R$  

$V_3 = V_4 = V_{AC} \cdot \frac{R}{R+R} = V_{AC} \cdot \frac{1}{2} = \frac{25.26}{2} = 12.63V$  
$I_3 = \frac{V_3}{R} = \frac{12.63}{4} = 3.1575A$  
$I_1 = I_2 + I_3 = 4.21 + 3.1575 = 7.37A$  

Calcoliamo ora la potenza del generatore e le potenze assorbite da ciascun resistore.  

$P_E = E \cdot I_1 = 40 \cdot 7.37 = 294.8W$  
$P_1 = V_1 \cdot I_1 = 14.74 \cdot 7.37 = 108.63W$  
$P_2 = V_2 \cdot I_2 = 25.26 \cdot 4.21 = 106.34W$  
$P_3 = V_3 \cdot I_3 = P_4 = V_4 \cdot I_3 = 12.63 \cdot 3.1575 = 39.88W$  

Verifichiamo il principio di conservazione dell'energia

$P_E = P_1 + P_2 + P_3 + P_4 = 108.63 + 106.34 + 39.88 + 39.88 \simeq 294.8W\ verificato \checkmark$


