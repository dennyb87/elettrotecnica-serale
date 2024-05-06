# Apertura-chiusura di una finestra di un'azienda zootecnica  

Si vuole progettare il sistema di controllo e azionamento della finestra di un'azienda zootecnica che, essendo di grandi dimensioni, necessita di motori per essere messa in movimento.  

## Requisiti  

> La finestra si apre/chiude alla pressione rispettivamente di un pulsante di apertura/chiusura ed e' mossa da un motore asincrono trifase.

> L'apertura/chiusura della finestra termina automaticamente quando questa e' completamente aperta/chiusa.

> In qualsiasi momento e' possibile interrompere il movimento della finestra premendo un pulsante di stop/emergenza.

## Modello  

![finestra_zootecnica_schema](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c5d05634-f811-4adf-ac28-c98c5d3edccd)  

Il sistema di controllo e' composto da tre pulsanti:
* $P_M$ (marcia)
* $P_I$ (inversione)
* $P_A$ (arresto)

Mentre per determinare lo stato delle finestre si hanno due finecorsa posti alle estremita' delle guide $F_1,\ F_2$ (vedi figura) che permettono l'abilitazione del motore.  

Per la segnalazione si hanno due lampade rispettivamente di marcia $L_M$ e inversione $L_I$. In caso di sovraccarico scatta il rele' termico $R_T$ che le accende entrambe indicando il malfuzionamento.  

| I/O   | componente             | simbolo  | ID      | stato iniziale | descrizione                                               |
| ----- | ---------------------- | -------- | ------- | -------------- | --------------------------------------------------------- |
| input | pulsante marcia        | $P_M$    | $I_1$   | 0              | 1 aziona la chiusura della finestra, 0 altrimenti         |
| input | pulstante inversione   | $P_I$    | $I_2$   | 0              | 1 aziona l'apertura della finestra, 0 altrimenti          |
| input | pulsante arresto       | $P_A$    | $I_3$   | 1              | 0 se la finestra e' in arresto, 1 altrimenti              |
| input | finecorsa              | $F_1$    | $I_4$   | 1              | 0 se la finestra e' totalmente chiusa, 1 altrimenti       |
| input | finecorsa              | $F_2$    | $I_5$   | 0              | 1 se la finestra e' totalmente aperta, 0 altrimenti       |
| out   | contattore marcia      | $K_1$    | $Q_1$   | 0              | 1 aziona il motore in marcia, 0 altrimenti                |
| out   | contattore  inversione | $K_2$    | $Q_2$   | 0              | 1 aziona il motore in inversione, 0 altrimenti            |
| out   | lampada marcia         | $L_M$    | $Q_3$   | 0              | 1 si accende lampanda di marcia, 0 altrimenti             |
| out   | lampada inversione     | $L_I$    | $Q_4$   | 0              | 1 si accende lampanda di inversione, 0 altrimenti         |
| out   | tutte le lampade       | $L_ML_I$ | $Q_3Q4$ | 0              | 1 accende tutte le lampade per sovraccarico, 0 altrimenti |

## Schemi di potenza e controllo  

![finestra_zootecnica](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/26178df4-672a-4d2e-896d-c12876b792b9)  
