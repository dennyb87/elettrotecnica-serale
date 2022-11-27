# Analisi dei circuiti e verifica dei Principi di Kirchhoff  

![c02_fig1](https://user-images.githubusercontent.com/7195133/204142919-0fe46edf-533b-4584-be1b-d7b4e8358fe7.jpg)  
![c02_fig2](https://user-images.githubusercontent.com/7195133/204142935-9d361872-935a-4851-a9ae-e635a3f1e3e6.jpg)


## 1. Struttura del circuito
Nel circuito si hanno:
- 7 componenti (3 generatori, 4 resistori) e 2 collegamenti a resistenza nulla;
- 6 punti di connessione; i punti di connessione sono $A, B, C, D, F, G$
- n = 5 nodi; i nodi sono $A, B, C, D, F$
- r = 8 rami; in tutti i rami si ha un solo componente eccetto il ramo che collega i nodi B,
C dove i componenti sono in serie
- i rami che collegano i nodi A, B e i nodi A, D: tali rami hanno resistenza nulla
- in ogni ramo scorre una corrente; le correnti di ramo sono individuate da un verso (scelto
arbitrariamente) e da un nome.  


Si hanno quindi 4 maglie indipendenti visto che $m_{indipendenti}=r-n+1$ infatti $4 = 8 - 5 + 1$  

## 2. Calcolo delle tensioni tra i punti di connessione consecutivi  

Tra due qualsiasi punti di connessione consecutivi del circuito si ha tensione.
La tensione può essere calcolata in uno dei seguenti modi tenendo conto del  
componente presente tra i due punti considerati.  

In particolare
a) se c’è un generatore di tensione la tensione è un dato del circuito;
b) se c’è un collegamento a resistenza nulla la tensione è 0;
c) se c’è una resistenza e si conosce la corrente la tensione può essere calcolata applicando la
legge di Ohm.
Nei casi a) , c) la tensione può essere positiva o negativa a seconda dell’ordine con cui è calcolata.

|                                               |                  |
| --------------------------------------------- | ---------------- |
| $V_{AB} = 0V$                                 | Resistenza nulla |
| $V_{FA} = E_1 = 10V$                          | Generatore       |
| $V_{FB} = R_2 \cdot I_2 = 4 \cdot 2.5 = 10V$  | Legge di Ohm     |
| $V_{FC} = -E_2 = -20V$                        | Generatore       |
| $V_{FD} = R_1 \cdot I_1 = 2 \cdot 5 = 10V$    | Legged di Ohm    |
| $V_{DF} = -R_1 \cdot I_1 = -2 \cdot 5 = -10V$ | Legge di Ohm     |
| $V_{CD} = R_3 \cdot I_3 = 6 \cdot 5 = 30V$    | Legge di Ohm     |
| $V_{GB} = R_4 \cdot I_4 = 8 \cdot 0 = 0V$     | Legge di Ohm     |
| $V_{DA} = 0V$                                 | Resistenza nulla |
| $V_{FA} = E_1 = 10V$                          | Generatore       |
| $V_{CF} = E_2 = 20V$                          | Generatore       |
| $V_{GC} = -30V$                               | Generatore       |


## 3. Verifica del Primo Principio di Kirchhoff (IPK)  

| Nodo    | IPK                     | Calcolo                                       | Verificato   |
| ------- | ----------------------- | --------------------------------------------- | ------------ |
| $1 - A$ | $I_7 + I_8 = I_6$       | $I_7 + I_8 = 10 + 2.5 = I_6 = 12.5A$          | $\checkmark$ |
| $2 - B$ | $I_2 + I_4 = I_8$       | $I_2 + I_4 = 2.5 + 0 = I_8 = 2.5A$            | $\checkmark$ |
| $3 - C$ | $I_4 + I_3 = I_5$       | $I_4 + I_3 = 0 + 5 = I_5 = 5V$                | $\checkmark$ |
| $4 - D$ | $I_1 + I_3 = I_7$       | $I_1 + I_3 = 5 + 5 = I_7 = 10V$               | $\checkmark$ |
| $5 - F$ | $I_2 + I_3 + I_1 = I_6$ | $I_2 + I_3 + I_1 = 2.5 + 5 + 5 = I_6 = 12.5V$ | $\checkmark$ |
