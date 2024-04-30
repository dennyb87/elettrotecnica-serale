# Apertura-chiusura di una finestra di un'azienda zootecnica  

Si vuole progettare il sistema di controllo e azionamento della finestra di un'azienda zootecnica che, essendo di grandi dimensioni, necessita di motori per essere messa in movimento.  

## Requisiti  

> La finestra si apre/chiude alla pressione rispettivamente di un pulsante di apertura/chiusura ed e' mossa da un motore asincrono trifase.

> L'apertura/chiusura della finestra termina automaticamente quando questa e' completamente aperta/chiusa.

> In qualsiasi momento e' possibile interrompere il movimento della finestra premendo un pulsante di stop/emergenza.

## Modello  

![control_panel](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9a1bde05-4ee8-4c0b-bc2e-a8611d91bd0d)  

Il sistema di controllo sara' composto da tre pulsanti:
* $P_M$ (marcia)
* $P_I$ (inversione)
* $P_A$ (arresto)

![finestra_zootecnica](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a1024dce-49e5-44a5-b1ca-c49d8ed72ffd)  

Per determinare lo stato delle finestre si avranno due finecorsa posti alle estremita' delle guide $F_1,\ F_2$ (vedi figura)  

| I/O   | componente             | simbolo | ID    | stato iniziale | descrizione                                       |
| ----- | ---------------------- | ------- | ----- | -------------- | ------------------------------------------------- |
| input | pulsante marcia        | $P_M$   | $I_1$ | 0              | 1 aziona la chiusura della finestra, 0 altrimenti |
| input | pulstante inversione   | $P_I$   | $I_2$ | 0              | 1 aziona l'apertura della finestra, 0 altrimenti  |
| input | pulsante arresto       | $P_A$   | $I_3$ | 1              | 0 se la finestra e' in arresto, 1 altrimenti      |
| input | finecorsa              | $F_1$   | $I_4$ | 1              | 0 se la finestra e'chiusa, 1 altrimenti           |
| input | finecorsa              | $F_2$   | $I_5$ | 0              | 1 se la finestra e' aperta, 0 altrimenti          |
| out   | contattore marcia      | $K_1$   | $Q_1$ | 0              | 1 se la bobina e' eccitata, 0 altrimenti          |
| out   | contattore  inversione | $K_2$   | $Q_2$ | 0              | 1 se la bobina e' eccitata, 0 altrimenti          |
| out   | lampada marcia         | $L_M$   | $Q_3$ | 0              | 1 se la lampada e' accesa, 0 altrimenti           |
| out   | lampada inversione     | $L_I$   | $Q_4$ | 0              | 1 se la lampada e' accesa, 0 altrimenti           |