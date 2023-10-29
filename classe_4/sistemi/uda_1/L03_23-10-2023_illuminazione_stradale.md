# Illuminazione stradale  

> L'illuminazione avviene mediante l'accensione di lampioni, questa puo' essere fatta manualmente, oppure con un timer ed un sensore di luce

## Identificazione variabili di input  

| nome         | simbolo | tipo    | stati                                                  |
| ------------ | ------- | ------- | ------------------------------------------------------ |
| interruttore | INT     | binario | $$0 \implies aperto \\ 1 \implies chiuso$$             |
| sensore      | SL      | binario | $$0 \implies buio \\ 1 \implies luce$$                 |
| timer        | T       | binario | $$0 \implies\ fuori\ fascia \\ 1 \implies in\ fascia$$ |

```mermaid
flowchart TB
   start(["start"])-->readint["read INT"]
   readint-->inton{"INT on ?"}
   inton-->|Yes| lampson{"street lamps on ?"}
   lampson-->|Yes| start
   lampson-->|No| turnlampson["turn lamps ON"]
   turnlampson-->start
   inton-->|No| readtimer["read T"]
   readtimer--> timeron{"T on ?"}
   timeron-->|Yes| readsensor["read SL"]
   timeron-->|No| lampson2
   readsensor-->sensoron{"S on ?"}
   sensoron-->|No| lampson
   sensoron-->|Yes| lampson2{"street lamps on ?"}
   lampson2-->|No| start
   lampson2-->|Yes| turnlampsoff["lamps OFF"]
   turnlampsoff-->start
```
