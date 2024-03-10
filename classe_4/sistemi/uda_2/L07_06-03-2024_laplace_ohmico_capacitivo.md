# Circuito ohmico-capacitivo nel dominio di Laplace  

![ohmico-capacitivo_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/d51147b8-c487-4ed1-a00f-22352a73f2e0)  

Come gia' accennato per poter risolvere questo tipo di circuiti e' necessario passare al dominio di Laplace per poter operare su frazioni algebriche in modo da evitare equazioni differenziali. Si ha allora che:  

$e(t) = 40u(t) \implies E(s) = \dfrac{40}{s}$  

$X_c = \dfrac{1}{Cs} = \dfrac{1}{0.08s}$  

A questo punto e' possibile risolvere il circuito sfruttando la legge di Ohm.  

$Z_{tot} = R + X_c = R + \dfrac{1}{Cs} = \dfrac{RCs+1}{Cs}$  

$I(s) = \dfrac{E(s)}{Z_{tot}} = E(s) \cdot \dfrac{Cs}{RCs+1} = \dfrac{E(s)Cs}{RCs+1}$  

$V_R = R \cdot I(s) = R \cdot \dfrac{E(s)Cs}{RCs+1}$  

$V_c(s) = X_c \cdot I(s) = \dfrac{1}{\cancel{Cs}} \cdot \dfrac{E(s)\cancel{Cs}}{RCs+1} = \dfrac{E(s)}{RCs+1}$  

Si vuole ora trovare la funzione di trasferimento...  

$G(s) = \dfrac{V_c(s)}{E(s)} = \dfrac{\cancel{E(s)}}{RCs+1} \cdot \dfrac{1}{\cancel{E(s)}} = \dfrac{1}{RCs+1}$  

Questo risultato, che avremmo potuto ottenere anche con il partitore di tensioni ci mostra un fatto:  

> le funzioni di trasferimento non dipendono dagli input, ma dalla composizione del sistema stesso!

## Ritorno al dominio del tempo  

Vogliamo ora esaminare il comportamento di tensione e corrente nel tempo per cui occorre tornare nel dominio del tempo, ma per farlo e' necessario manipolare la frazione algebrica per permettere l'antitrasformata.  

$I(s) = E(s) \cdot \dfrac{Cs}{RCs+1} = \dfrac{40}{\cancel{s}} \cdot \dfrac{0.08\cancel{s}}{5\cdot0.08 \cdot s+1} = \dfrac{3.2}{0.4s+1}$  

$I(s) = 3.2 \cdot \dfrac{1}{0.4\bigg(s+\frac{1}{0.4}\bigg)} = \dfrac{3.2}{0.4} \cdot \dfrac{1}{s+\frac{1}{0.4}}$  

$i(t) = 8 \cdot e^{-0.4t} \cdot u(t)$  

![vi_graph_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/8541baeb-50c8-4408-960d-531026f64e54)  

Osservando il grafico e' possible notare come il nostro risulato sia in accordo con le grandezze misurate nel simulatore. In particolare la corrente (in blu) e' al suo massimo all'istante $t = 0s$ dove la tensione (in verde) e' invece $0\ V$.  
