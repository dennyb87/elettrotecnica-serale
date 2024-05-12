# Risposta in frequenza  

Al contrario dei resistori che, nel caso caso ideale, sono componenti la cui resistenza e' costante nel tempo al variare della frequenza, i **condensatori** e i **capacitori** cambiano il loro comportamento in dipendenza della *frequenza*. Lo studio di questo comportamento prende il nome di **risposta in frequenza**, ovvero lo studio di come il sistema cambi la propria configurazione, e quindi il comportamento, in dipendenza della frequenza.  

![componente_frequency_reponse](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f1d38550-4c21-4c6e-acf6-3b34f8632305)  

Prendendo in considerazione i casi limite, si ottiene la seguente tabella.  

| $Z$   | $Z$                   | $Z\vert_{\omega=0}$ | $Z\vert_{\omega=\infty}$ |
| ----- | --------------------- | ------------------- | ------------------------ |
| $R$   | $R$                   | $R$                 | $R$                      |
| $X_L$ | $\omega L$            | $0$                 | $\infty$                 |
| $X_C$ | $\dfrac{1}{\omega C}$ | $\infty$            | $0$                      |

in definitiva, la risposta in frequenza del sistema non e' che la funzione di trasferimento, calcolata con la frequenza in esame.  

$G(s)\bigg\vert_{s = j\omega} = \dfrac{Y(s)}{X(s)}$  
