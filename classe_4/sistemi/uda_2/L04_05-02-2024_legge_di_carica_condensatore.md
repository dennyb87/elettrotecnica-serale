# Legge di carica di un condensatore  

![capacitor_charge_curve](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/297bb7c1-ad26-4315-945b-49e8cde2b495)  

Si vuole rendere nota senza dimostrazione l'equazione per la tensione sul condensatore in fase di carica.  

$v(t) = \bigg[V_f + (V_i - V_f) \cdot e^{-\frac{t}{\tau}} \bigg] \cdot u(t)$  

Dove $u(t)$ e' la fuzione a gradino di cui ci serviamo per prendere in considerazione solo valori per $t$ maggiore di zero, mentre $e$ e' il numero di *Eulero*, costante matematica approssimabile a $2.71$.  

Siamo allora di fronte ad una funzione esponeziale, ovvero una funzione data da una potenza con base costante ed esponente variabile. Si fa' presente che in caso di scarica la funzione resta la stessa, a variare sono solo la tensione iniziale $V_i$ e quella finale $V_f$. Verifichiamo due casi particolari:  

$v(0) = \bigg[V_f + (V_i - V_f) \cdot e^0 \bigg] \cdot \cancel{1}$  

$v(0) = \bigg[V_f + (V_i - V_f) \cdot \cancel{1} \bigg]$  

$v(0) = \cancel{V_f} + V_i - \cancel{V_f} = V_i$  

Con $t = 0\ s$ otteniamo la tensione iniziale $V_i$ mentre con $t\to\infty$ quella finale $V_f$  

$\underset{t\to\infty}{v(t)} = \bigg[V_f + \cancel{(V_i - V_f) \cdot 0} \bigg] \cdot \cancel{1} = V_f$   

## Transitori nei sistemi del primo ordine  

La funzione e' valida per ogni sistema di primo ordine, ovvero quei sistemi in cui e' presente solo un componente in grado di immagazzinare energia. Questa descrive il comportamento del sistema durante un transitorio, ovvero il tempo che intercorre tra due stati di regime stazionario. Per **regime stazionario** si intende non solo quando il sistema non varia il suo funzionamento nel tempo, ma anche nei casi in cui e' presente una variazione periodica e.g. regime sinusoidale.  

![tangent_tau](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1bb3ffb2-e691-40c3-afe2-c09ee35c570c)  

Si fa presente che tracciando la tangente di $v(t)$ all'istante $t = 0\ s$ questa individua proprio $\tau$ all'intersezione con l'asse delle ascisse.  
