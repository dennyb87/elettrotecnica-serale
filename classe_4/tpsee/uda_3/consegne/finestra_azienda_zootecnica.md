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

![finestra_zootecnica](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/74b5c6b7-6f74-4a67-901c-a238335d9009)  



Per determinare lo stato delle finestre si avranno due finecorsa posti alle estremita' delle guide (vedi figura) dove:  

* $F_1$ (normalmente chiuso **NC**)
* $F_2$ (normalmente aperto **NO**)

| I/O   | nome  | ID    | stato iniziale |
| ----- | ----- | ----- | -------------- |
| input | $P_M$ | $I_1$ |                |
| input | $P_I$ | $I_2$ |                |
| input | $P_A$ | $I_3$ |                |
