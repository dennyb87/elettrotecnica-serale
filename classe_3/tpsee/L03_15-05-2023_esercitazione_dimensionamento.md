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