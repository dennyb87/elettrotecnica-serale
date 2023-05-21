# Esercitazione dimensionamento  

```mermaid
graph TD
    contatore-.->magnetotermico--"25m PVC 1 linea esistente"-->QEG
    QEG-.->prese["10 prese 2P+T 16A"]
    QEG-.->lampade["10 lampade 35W"]
    QEG-.->clima["AirCon 1.5kW"]
```

Tenendo conto che siamo all'interno di un ufficio vogliamo determinare:  

1. la potenza convenzionale complessiva
2. la tipologia e sezione della linea di alimentazione del quadro elettrico
3. il magnetotermico differenziale generale (si consideri la resistivita' del suolo $\rho_E = 300\ \Omega m$ e che nel quadro sono presenti differenziali da $30\ mA$)


## Potenza convenzionale e corrente d'impiego  

$P_{prese} = N \cdot V_{n} \cdot I_{max} \cdot \cos \varphi \cdot K_p = 10 \cdot 230 \cdot 16 \cdot 0.9 \cdot 0.1 = 3312\ W$  

$P_{luci} = N \cdot P_n \cdot K_p \cdot K_c = 10 \cdot 35 \cdot 1 \cdot 0.8 = 280\ W$  

$P_{aircon} = \dfrac{P_n}{\eta} \cdot K_u \cdot K_c = \dfrac{1500}{0.9} \cdot 0.8 \cdot 1 \simeq 1333\ W$  

Si ha allora che la potenza convenzionale e':  

$P_c = P_{prese} + P_{luci} + P_{aircon} = 3312 + 280 + 1333 = 4925\ W$  

Troviamo ora la corrente d'impiego.  

$I_b = \dfrac{P_c}{V_n \cdot \cos \varphi} = \dfrac{4925}{230 \cdot 0.9} \simeq 23.8\ A$  


## Dimensionamento linea (portata)  

Sappiamo che la portata $I_z$ deve soddisfare la condizione:  

$I_b \le I_z$  

Considerando la posa **3A** in aria si assumera' una temperatura di $30^\circ$ quindi $K_1 = 1$ ed un $K_2 = 0.8$ che tiene conto di una posa a fascio con una linea esistente. Ipotizzando il caso peggiore dove $I_b = I_z = I_0 \cdot K_1 \cdot K_2$ si ha allora che:  

$I_0 = \dfrac{I_b}{K_1 \cdot K_2} = \dfrac{23.8}{0.8} = 29.75\ A$  

![posa_esercizio_tpsee_uda3](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/69b62a33-6b2c-4d25-9ed3-2084c735f4b8)  

Per soddisfare $I_0 \ge 29.75\ A$ si sceglie allora una cavo di sezione $4\ mm^2$ con $I_0 = 30\ A$.    


## Dimensionamento linea (caduta di tensione)  

Decidiamo che per questa linea si puo' avere una caduta di tensione massima del 2% ovvero $4.6\ V$.  

$u = \dfrac{\Delta V \cdot 1000}{I_b \cdot L} = \dfrac{4.6 \cdot 1000}{23.8 \cdot 25} \simeq 7.73\ \frac{mV}{Am}$  

![caduta_tensione_tpsee_uda3](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cf0e154a-7a0f-45a8-b01b-fd94912faaef)  

Si considera allora la caduta di tensione minore di quella calcolata ovvero $7.19\ \frac{mV}{Am}$ trovando che la sezione di $4\ mm^2$ calcolata in funzione della portata non va bene, ma ci serve invece una sezione di $6\ mm^2$.  
