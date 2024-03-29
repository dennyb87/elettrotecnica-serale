# Nastro trasportatore  

![nastro_trasportatore](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/246c4a6c-97a3-407b-b0ea-d41dd66ad9c8)  

> Alla pressione del pulsante di marcia il nastro trasportatore si attiva. Quando l'oggetto raggiunge la fine del nastro, questo deve fermarsi anche se il pulsante di marcia e' premuto.  

## Lista componenti  

| componente        | simbolo | note                                          | stati                             |
| ----------------- | ------- | --------------------------------------------- | --------------------------------- |
| pulsante          | PM      | pulsante marcia NO                            | 0/1 - premuto/altrimenti          |
| sensore posizione | SP      | segnala presenza oggetto a fine corsa         | 1/0 - oggetto presente/altrimenti |
| nastro            | BELT    | muove l'oggetto ruotando grazie alla puleggia | 1/0 - acceso/spento               |

```mermaid
flowchart TB
    start(["start"])-->readsp["read SP"]
    readsp-->spon{"SP on ?"}
    spon-->|Yes| readbelt["read BELT"]
    readbelt-->belton{"BELT on ?"}
    belton-->|Yes| switchbeltoff["BELT OFF"]
    switchbeltoff-->start
    belton-->|No| start

    spon-->|No| readpm["read PM"]
    readpm-->pmon{"PM on ?"}
    pmon-->|No| start
    pmon-->|Yes| switchbelton["BELT ON"]
    switchbelton-->start
```