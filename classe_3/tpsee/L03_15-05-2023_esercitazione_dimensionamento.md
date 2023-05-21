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
3. il magnetotermico differenziale generale (si consideri la resistivita' del suolo $\rho_E = 300\ \Omega m$ e che nel quadro sono presenti differenziali da $30 \mA$)


