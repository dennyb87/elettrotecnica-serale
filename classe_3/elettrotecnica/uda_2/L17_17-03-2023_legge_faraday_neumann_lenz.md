# Legge di Faraday-Neumann-Lenz  

![faraday_law_induction](https://user-images.githubusercontent.com/7195133/226195806-5fe0ca41-591c-4919-9dca-16ee252db56c.gif)


E' sperimentabile che posto un magnete immobile nei pressi o all'interno di una spira collegata ad un voltmetro, non si presenta nessun fenomeno osservabile. Nel momento in cui questo magnete viene messo in movimento si puo' osservare una tensione indotta nella spira. Questa tensione risulta essere uguale alla variazione di flusso nel tempo. Questo fatto e' stato formalizzato come segue:  

$v = - \dfrac{\Delta \phi}{\Delta t}$  

Il segno ci dice che la tensione indotta genera una corrente in un verso tale da produrre un campo magnetico che si oppone alla variazione di flusso che lo ha generato. Quindi conoscendo per esempio il campo e la direzione in cui si muove possiamo sempre derivare il campo indotto in quanto sara' quel campo che si oppone al movimento del primo, e di conseguenza possiamo dedurre anche il verso della corrente che lo ha generato.  

![faraday_law_induction_example](https://user-images.githubusercontent.com/7195133/226990274-a23033b1-b9d7-4fb4-b503-1a92b3f7e414.jpg)  

Vogliamo ora calcolare la tensione indotta prendendo come riferimento lo scenario in figura ma supponendo di avere una singola spira. Tracciando l'andamento del flusso nel tempo si otterrebbe un grafico di questo tipo.  

![flux_over_time](https://user-images.githubusercontent.com/7195133/227022324-349069eb-272d-4e17-aab5-1994d054f3d2.jpg)  

Possiamo dedurre dal grafico che il magnete si muove a velocita' costante verso la spira, infatti vediamo il flusso aumentare.  

$\Delta \phi_1 = \phi_f - \phi_i = 25 - 10 = 15\ mW$  

$\Delta t_1 = t_f - t_i = 5 - 0 = 5\ ms$  

$v = - \dfrac{\Delta \phi_1}{\Delta t_1} = - \bigg(\dfrac{15 \cdot \cancel{10^{-3}}}{5\cdot \cancel{10^{-3}}}\bigg) =  -3\ V$  

A questo punto si ferma per qualche secondo, ed il flusso resta quindi costante.  

$\Delta \phi_2 = \phi_f - \phi_i = 25 - 25 = 0\ mW$  

$\Delta t_2 = t_f - t_i = 7 - 5 = 2\ ms$  

$v = - \dfrac{\Delta \phi_2}{\Delta t_2} = - \bigg(\dfrac{0}{2}\bigg) = 0\ V$  

Infine vediamo il magnete allontanarsi sempre a velocita' costante raggiungendo un punto in cui l'effetto sulla spira e' zero, quindi piu' lontano del punto di partenza.  

$\Delta \phi_3 = \phi_f - \phi_i = 0 - 25 = -25\ mW$  

$\Delta t_3 = t_f - t_i = 10 - 7 = 3\ ms$  

$v = - \dfrac{\Delta \phi_3}{\Delta t_3} = - \bigg(- \dfrac{25 \cdot \cancel{10^{-3}}}{3 \cdot \cancel{10^{-3}}}\bigg) = 8.33\ V$  
