# Cablaggio PLC  

![schema_cablaggio_plc](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/3c5e0822-c378-4126-a5c2-bf07dec5cd71)  

Il PLC deve essere alimentato opportunamente alimentato, ad esempio a 24V, per cui si utilizzando gli appositi morsetti fase e neutro (F/N in figura).  

Nella parte superiore, oltre all'alimentazione, si hanno i morsetti di input, per cui ogni sensore, pulsante etc.. verra' qui opportunamente collegato. Il PLC riesce quindi atttraverso la presenza/assenza di tensioni sulle relative resistenze, a sfruttare la logica programmata per aggiornare gli stati di output in basso.  

Il PLC non supporta grandi tensioni per cui nel caso della marcia/arresto di un motore le uscite vanno a comandare un contattore che a sua volta chiudera' un circuito di potenza.  

## INPUT  

| VAR   | SIMBOLO | VALORE INIZIALE | NOTE                      |
| ----- | ------- | --------------- | ------------------------- |
| $I_0$ | PM      | 0               | Pulsante di marcia NO     |
| $I_1$ | PA      | 1               | Pulsante di arresto NC    |
| $I_2$ | RT      | 1               | Contatto rele' termico NC |

## OUTPUT  

| VAR   | SIMBOLO | VALORE INIZIALE | NOTE                                      |
| ----- | ------- | --------------- | ----------------------------------------- |
| $Q_0$ | KM      | 0               | Bobina contattore                         |
| $Q_1$ | LF      | 1               | Lampada fermo                             |
| $Q_2$ | LM      | 0               | Lampada    marcia                         |
| $Q_3$ | LRT     | 0               | Lampada          intervento rele' termico |
