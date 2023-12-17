# Progetto previsioni meteo  

Si vogliono trovare le equazioni di uscita per un circuito in grado di segnalare se il tempo migliorera', rimarra' stabile, o peggiorera'. Le variabili di ingresso binarie sono: pressione **P**, umidita' **U**, vento **V**, temperatura **T**, per le quali un 1 indica un aumento e uno 0 indica una diminuzione. Le uscite sono invece individuate da: bello $Y_B$, stabile $Y_S$, cattivo $Y_C$.  

## Modello predittivo  

* con aumenti di pressione si prevede bel tempo, a meno che la velocita' del vento non superi 20km/h, in tal caso si prevedono condizioni stabili
* una diminuzione di pressione con aumento di umidita' indica un peggioramento
* una diminuzione di pressione con vento superiore a 20km/h indica un peggioramento; se pero' la temperatura si innalza le condizioni rimarranno stabili
* in tutti gli altri casi le condizioni rimangono stabili

Scriviamo allora le equazioni preliminari del modello:  

$Y_B = P\overline{V}$  
$Y_C = \overline{P}U + \overline{P}V\overline{T}$  
$Y_S = \overline{Y_B + Y_C}$  

Possiamo semplificare le uscite ignorando $Y_S$ in quanto il tempo si puo' considerare stabile ogni volta che le predizioni $Y_B$ e $Y_C$ non si verificano.  

## Individuazione delle variabili  

| variabile binaria | stato                   | livello logico |
| ----------------- | ----------------------- | -------------- |
| P                 | aumento pressione       | 1              |
|                   | diminuzione pressione   | 0              |
| U                 | aumento umidita'        | 1              |
|                   | diminuzione umidita'    | 0              |
| V                 | amuento vento           | 1              |
|                   | diminuzione vento       | 0              |
| T                 | aumento tempratura      | 1              |
|                   | diminuzione temperatura | 0              |

## Tabella di verita'  

| idx | P   | U   | V   | T   | $Y_B$ | $Y_C$ |
| --- | --- | --- | --- | --- | ----- | ----- |
| 0   | 0   | 0   | 0   | 0   | 0     | 0     |
| 1   | 0   | 0   | 0   | 1   | 0     | 0     |
| 2   | 0   | 0   | 1   | 0   | 0     | 1     |
| 3   | 0   | 0   | 1   | 1   | 0     | 0     |
| 4   | 0   | 1   | 0   | 0   | 0     | 1     |
| 5   | 0   | 1   | 0   | 1   | 0     | 1     |
| 6   | 0   | 1   | 1   | 0   | 0     | 1     |
| 7   | 0   | 1   | 1   | 1   | 0     | 1     |
| 8   | 1   | 0   | 0   | 0   | 1     | 0     |
| 9   | 1   | 0   | 0   | 1   | 1     | 0     |
| 10  | 1   | 0   | 1   | 0   | 0     | 0     |
| 11  | 1   | 0   | 1   | 1   | 0     | 0     |
| 12  | 1   | 1   | 0   | 0   | 1     | 0     |
| 13  | 1   | 1   | 0   | 1   | 1     | 0     |
| 14  | 1   | 1   | 1   | 0   | 0     | 0     |
| 15  | 1   | 1   | 1   | 1   | 0     | 0     |

## Somme di mintermini  

$Y_B = m_8 + m_9 + m_{12} + m_{13} = P\overline{UVT} + P\overline{UV}T + PU\overline{VT} + PU\overline{V}T$  

$Y_C = m_2 + m_4 + m_5 + m_6 + m_7 = \overline{PU}V\overline{T} + \overline{P}U\overline{VT} + \overline{P}U\overline{V}T + \overline{P}UV\overline{T} + \overline{P}UVT$  

## Mappa di Karnaugh $Y_B$  

| VT-PU  | 00  | 01  | 11  | 10  |
| ------ | --- | --- | --- | --- |
| **00** |     |     | 1   | 1   |
| **01** |     |     | 1   | 1   |
| **11** |     |     |     |     |
| **10** |     |     |     |     |

$Y_B = P\overline{V}$  

Si noti che il risultato coincide con l'equazione preliminare.  

## Mappa di Karnaugh $Y_C$  

| VT-PU  | 00  | 01  | 11  | 10  |
| ------ | --- | --- | --- | --- |
| **00** |     | 1   |     |     |
| **01** |     | 1   |     |     |
| **11** |     | 1   |     |     |
| **10** | 1   | 1   |     |     |

$Y_C = \overline{P}U + \overline{P}V\overline{T}$  

Anche in questo caso la forma minima coincide con l'equazione preliminare che evidentemente non era ulteriormente semplificabile.  

## Schema circuito  

![schema_circuito_logico](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a543536c-caec-4873-94f5-073b9bbbce58)  

## Implementazione in Tinkercad  

Vedi nel [simulatore](https://www.tinkercad.com/things/7KqlqGTxMNT-fad-uda1-2023-previsioni-meteo)  

![tinkercad_weather_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/011e4459-13f1-4da1-9e52-11f3f6d33f66)  