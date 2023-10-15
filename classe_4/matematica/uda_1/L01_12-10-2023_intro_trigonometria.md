# Intro trigonometria  

La trigonometria studia i triangoli a partire dai loro angoli, e permette grazie a misure note di calcolare tutte le altre, ovvero di eseguire la *risoluzione dei triangoli*. Due semirette uscenti dallo stesso punto (vertice) formano due angoli:  

* **convesso** $\lt 180^\circ$ non contiene il prolungamento dei lati
* **concavo** $\gt 180^\circ$ contiene il prolungamento dei lati

![angolo_convesso_concavo](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/e68ef120-67cf-4a30-97c1-944e48d9d2df)  

Si dice invece:  

* **piatto** se e' uguale a $180^\circ$
* **retto** se e' uguale a $90^\circ$
* **giro** se e' uguale a $360^\circ$

![angoli_supplementari](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/303ef9df-b180-40d6-beef-b850fd86aa51)  

Due angoli si dicono:

* **complementari** se $\alpha + \beta = 90^\circ$
* **supplementari** se $\alpha + \beta = 180^\circ$
* **esplementari** se $\alpha + \beta = 360^\circ$

# Circonferenza goniometrica  

![unit_circle](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/2ccab7d8-a60b-4e9d-a674-3622ea5487f9)  

E' una circonferenza di raggio unitario centrata all'origine di un piano cartesiano, che come vedremo, ci permette di dedurre delle proprieta' valide per qualunque triangolo.  

Per convenzione si hanno angoli positivi in senso antiorario, e negativi in senso orario. Se l'angolo e' maggiore di $360^\circ$ significa che e' stato fatto piu' di un giro. In generale e' possibile scrivere:  

$\alpha = K \cdot 360^\circ$  

$900^\circ = 2.5 \cdot 360^\circ$  

Dove $K$ e' il numero di giri, oppure in modo equivalente...  

$\alpha = n \cdot 360^\circ + \beta$  

Dove $n$ e' il **numero intero** di giri, mentre $\beta$ e' l'angolo visibile nella circonferenza goniometrica.  

$900^\circ = 2 \cdot 360^\circ + 180^\circ$  

## Radiante  

![radiante](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/6a5f55ae-7cda-4981-bda6-75dcbf33fc58)  

Per definizione il radiante e' il rapporto tra un arco di circonferenza ed il suo raggio. Ne segue a parita' di angolo il rapporto sia indipendente dal raggio...  

$\alpha = \dfrac{l}{r} = \dfrac{l_1}{r_1}$  

Allora conoscendo la formula della circonferenza, e assumendo un cerchio di raggio unitario ne deriva che...  

$C = 2\pi r = 2\pi \cdot 1 \implies 2\pi = 360^\circ \implies \pi = 180^\circ$  

Essendo gradi e radianti proporzionali e' possibile quindi, dato un angolo misurato in radianti, trovare la misura equivalente in gradi e viceversa.  

$\dfrac{\alpha}{90^\circ} = \dfrac{2\pi}{360} \implies  \alpha = \dfrac{\cancel{2}\pi \cdot \cancel{90^\circ}}{\cancel{360^\circ}_2} =  \dfrac{\pi}{2}$  

$\dfrac{\beta}{\frac{1}{9}\pi} = \dfrac{180^\circ}{\pi} \implies \beta = \dfrac{\frac{1}{\cancel{9}}\cancel{\pi} \cdot \cancel{180^\circ}^{20}}{\cancel{\pi}} = 20^\circ$  

# Grado sessadecimale  

In questo sistema di numerazione in base $60$ l'unita' continua ad essere il grado, mentre i primi sono $\frac{1}{60}$ di grado, ed i secondi $\frac{1}{3600}$ di grado. Per la conversione si procede quindi come segue:  

$30^\circ\ 2^\prime\ 27^{\prime\prime} = 30^\circ + \dfrac{2}{60} + \dfrac{27}{3600} \simeq 30.0408^\circ$  

Con il procedimento inverso...  

$30.0408^\circ$  

$0.0408 \cdot 60 = 2.448^\prime$  

$0.448 \cdot 60 = 26.88^{\prime\prime} \simeq 27^{\prime\prime}$  

Arrotondando si ottiene infine di nuovo $30^\circ\ 2^\prime\ 27^{\prime\prime}$  
