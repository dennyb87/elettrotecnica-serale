# Movimentazione oggetto su nastro trasportatore temporizzato  

Alla pressione di un pulsante di marcia avanti, il pezzo viene mosso sul nastro trasportatore da un punto **A** ad un punto **B**. Raggiunta la posizione centrale **C** il pezzo si ferma per $10\ s$ per poi ripartire automaticamente e raggiungere la posizione finale **B** dove il pezzo si ferma definitivamente in attesa di essere tolto dal nastro. Sono previsti:  

* un pulsante di stop/emergenza che arresta il processo in qualunque momento
* un sensore di sovraccarico
* un sistema di segnalazione che indichi lo stato del processo

```mermaid
flowchart TB
    start(start)

    start-->readmat[leggi nastro]
    readmat-->mat{nastro in movimento ?}
    mat--NO-->readsc[leggi Pulsante MARCIA]
    readpm-->pm{PM premuto ?}
    pm--SI-->activatemat[aziona nastro]
    activatemat-->start

    mat--SI-->readps[leggi Pulsante STOP]
    readps-->ps{PS premuto}--SI-->stopmat[arresta nastro]
    stopmat-->start
    ps--NO-->readsc

    readsc[leggi sensore 1]
    readsc-->s1{sensore 1 attivato ?}
    s1--SI-->stopmat2[arresta nastro]-->readtime
    readtime[leggi tempo dall'attivazione]
    readtime-->timeended{tempo > 10 secondi ?}
    timeended--SI-->activatemat
    timeended--NO-->start

    s1--NO-->reads2[leggi sensore 2]
    reads2-->s2{sensore 2 attivato ?}
    s2--SI-->stopmat
    s2--NO-->readpm  
```