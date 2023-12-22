# Sistema di allarme  

Si deve progettare il sistema di allarme per un'abitazione. La casa e' dotata di una porta $P$ e due finestre $F_1$ ed $F_2$. Sulla porta e sulle finestre sono installati dei sensori che forniscono segnali con livello logico **ALTO** quando sono aperte e livello logico **BASSO** se sono chiuse. Si deve quindi far accendere una lampada di allarme $L$ ogni volta che si verificano le seguenti condizioni:  

* $P$ aperta ed $F_1$ e $F_2$ aperte
* $P$ aperta ed $F_1$ aperta
* $P$ chiusa ed $F_1$ e $F_2$ aperte

Vogliamo quindi trovare la funzione logica di uscita per $L$ e disegnare un possibile schema in linguaggio ladder.  

## Ipotesi aggiuntive  

$L = PF_1F_2 + \overline{P}F_1F_2 + PF_1$  
$L = F_1F_2 \cdot (P + \overline{P}) + PF_1$  
$L = F_1F_2 \cdot 1 + PF_1$  
$L = F_1F_2 + PF_1$  

$L = F_1 \cdot (F_2 + P)$  

Trovata la funzione logica di $L$ ci si accorge che il sistema, per come e' progettato, permette a finestre chiuse di aprire la porta senza far scattare l'allarme. Ignorando questo problema si ipotizza la presenza di un tastierino $T$ che controlla il sistema fornendo in uscita un livello logico **ALTO** quando il sistema di allarme e' attivo e **BASSO** quando non e' attivo. La funzione allora diventa:  

$L = F_1 \cdot (F_2 + P) \cdot T$  

## Lista di attribuzione  

| componente    | simbolo | ladder ID | stato iniziale | I/O    |
| ------------- | ------- | --------- | -------------- | ------ |
| fine corsa NO | $F_1$   | $I_1$     | 0              | input  |
| fine corsa NO | $F_2$   | $I_2$     | 0              | input  |
| fine corsa NO | $P$     | $I_3$     | 0              | input  |
| contatto NO   | $T$     | $I_4$     | 0              | input  |
| lampada       | $L$     | $Q_1$     | 0              | output |

## Cablaggo PLC e programma ladder  

![sistema_allarme_ladder_plc](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/e68bf1f7-d369-482b-923f-bbebd85905af)  

| rung | descrizione                                                                                                                                      |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| $R1$ | Singolo rung che gestisce la logica di attivazione della lampada e l'autoritenuta. L'interruzione avviene attraverso il tastierino di controllo. |
