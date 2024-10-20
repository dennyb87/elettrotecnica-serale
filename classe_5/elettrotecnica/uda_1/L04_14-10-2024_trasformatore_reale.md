# Trasformatore reale  

![real_transformer_circuit](https://github.com/user-attachments/assets/963943d3-00f4-4702-9fb5-50e26aca9096)  

Il circuito equivalente del trasformatore reale valido a basse frequenze e' essenzialmente quello del trasformatore ideale con dei componenti aggiuntivi che tengono conto delle perdite, questi componenti sono divisi in:  

* parametri longitudinali
* parametri traversali

### Parametri longitudinali  

Questi sono le **resistenze** in serie alle **reattanze induttive** $Z_1$ e $Z_2$ dove le resistenze tengono conto delle perdite nel rame degli avvolgimenti, mentre le reattanze tengono conto dei flussi dispersi, ovvero quella parte di flusso dispersa in aria che non riesce a raggiungere l'altro avvolgimento.  

### Parametri trasversali  

Questi sono i componenti aggiunti in parallelo e si riferiscono alle perdite del nucleo magnetico, dove $R_0$ tiene conto delle perdite nel ferro per isteresi e correnti parassite, mentre la reattanza induttiva $X_0$ tiene conto della riluttanza non nulla per cui c'e' bisogno di una corrente di magnetizzazione per creare il flusso.  

## Potenze in gioco  

$P_2 = V_2I_2\cos \varphi_2$  

La potenza reattiva in dipendenza del carico...  

$Q_2 = V_2I_2\sin \varphi_2$  

Potenza persa nel ferro $P_{fe}$ e nel rame $P_{cu}$  

$P_{fe} = \frac{1}{R_0}E_1^2$  

$P_{cu} = R_1I_1^2+R_2I_2^2$  

La potenza persa $P_P$...  

$P_P = P_{fe}+P_{cu}$  

Si ha allora che se $V_1$ e' la tensione in ingresso, la potenza persa e'...  

$P_1 = P_2 + P_P = V_1I_1\cos \varphi_1$  

Con $Q_T$ si identifica la potenza reattiva del trasformatore totale  

$Q_T = X_1I_1^2+X_2I_2^2+\frac{1}{X_0}E_1^2$  

Si ha infine che la potenza reattiva totale e'...  

$Q_1 = Q_T+Q_2$  
