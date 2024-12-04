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

### QE3 - Spogliatoio  

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

