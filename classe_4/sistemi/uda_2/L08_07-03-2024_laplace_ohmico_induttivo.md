# Circuito ohmico-induttivo nel dominio di Laplace  

![ohmico-induttivo_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c31987e4-ad1b-4165-8b1f-2d7fd634f04f)    

Per risolvere il circuito passiamo al dominio di Laplace.  

$e(t) = 20 \cdot u(t) \implies E(s) = \dfrac{20}{s}$  

$X_L = Ls = 0.5s$  

Procediamo a risolvere con la legge di Ohm.  

$Z_{tot} = R + Ls$  

$I(s) = \dfrac{E(s)}{Z_{tot}} = \dfrac{E(s)}{R+Ls}$  

$V_R = I(s) \cdot R = \dfrac{E(s)R}{R+Ls}$  

$V_L = I(s) \cdot X_L = I(s) \cdot Ls = \dfrac{E(s)Ls}{R+Ls}$  

Si vuole ora trovare la funzione di trasferimento...  

$G(s) = \dfrac{V_L(s)}{E(s)} = \dfrac{\cancel{E(s)}\ Ls}{R+Ls} \cdot \dfrac{1}{\cancel{E(s)}} = \dfrac{Ls}{R+Ls}$  

## Ritorno al dominio del tempo  

Per esaminare il comportamento di tensione e corrente nel tempo dobbiamo manipolare la frazione algebrica per permettere l'antitrasformata.  

$V_L(s) = \dfrac{E(s)Ls}{R+Ls} = \dfrac{20}{\cancel{s}} \cdot \dfrac{0.5\cancel{s}}{2+0.5s} = 20 \cdot \dfrac{0.5}{0.5\bigg(s+\frac{2}{0.5}\bigg)}$  

$V_L = 20 \cdot \dfrac{0.5}{0.5\bigg(s+\frac{2}{0.5}\bigg)} = \dfrac{10}{0.5} \cdot \dfrac{1}{s+4} \implies v_L(t) = 20 \cdot e^{-4t}\cdot u(t)$  

![vi_graph_02](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ddc93d48-74b3-4440-8682-d124b23f43ae)  

Al contrario del circuito capaticitivo, si ha tensione massima all'istante $t = 0s$ mentre la corrente e' $0\ A$. Questo e' dovuto alla tensione indotta sull'avvolgimento. La variazione di corrente causa una variazione di flusso che a sua volta produce una tensione opposta a quella che l'ha generata. Dopo un tempo $t$ abbastanza lungo la corrente arriva al suo massimo, e non essendoci piu' variazione di corrente anche la variazione di flusso magnetico cessa, ponendo fine alla tensione indotta. A questo punto l'induttore risulta cortocircuitato per cui la corrente deve essere:  

$I = \dfrac{E}{R} = \dfrac{20}{2} = 10\ A$  
