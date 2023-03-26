# Generatore elettrico 

![rotating_magnet_in_coil](https://user-images.githubusercontent.com/7195133/227459819-41008926-33df-43cf-ae15-b2b0fe861c46.gif)  

Andiamo ora ad esaminare il principio di funzionamento di un **generatore elettrico a magneti permanenti**. Sappiamo che la variazione di flusso magnetico nel tempo causa una tensione indotta in un conduttore nelle vicinanze. Vediamo allora cosa succede durante la rotazione di un magnete che produce un campo di induzione $B = 40\ mT$ (in quale punto dello spazio ?) all'interno di una spira di superficie $S = 400\ cm^2 = 400 \cdot 10^{-4}\ m^2 = 4 \cdot 10^{-2}\ m^2$.  

![rotating_magnet_in_coil](https://user-images.githubusercontent.com/7195133/227708033-bdb64975-6332-4099-8eb0-69aaeed93c4e.jpg)  

Si puo' notare che in posizione 1, 3 e 5 si ha un angolo $\alpha$ di $0^{\circ}$ gradi tra il campo di induzione e la superficie della spira, allora il flusso sara' zero.  

$\phi_1 = \phi_3 = \phi_5 = B \cdot S \cdot \cos \alpha = B \cdot S \cdot 0 = 0\ Wb$  

Si avra' invece un flusso massimo nelle posizioni 2 e 4 in quanto il campo di induzione e' normale alla superficie.  

$\phi_2 = B \cdot S \cdot \cos \alpha = 40 \cdot 10^{-3} \cdot 4 \cdot 10^{-2} \cdot 1 = 160 \cdot 10^{-5} = 1.6\ mWb$  

$\phi_4 = B \cdot S \cdot \cos \alpha = 40 \cdot 10^{-3} \cdot 4 \cdot 10^{-2} \cdot -1 = 160 \cdot 10^{-5} = -1.6\ mWb$  

Osserviamo cosa succede se tracciamo il flusso nel tempo.  

| $index$ | $t\ [ms]$ | $\phi\ [mWb]$ |
| ------- | --------- | ------------- |
| $1$     | $0$       | $0$           |
| $2$     | $5$       | $1.6$         |
| $3$     | $10$      | $0$           |
| $4$     | $15$      | $-1.6$        |
| $5$     | $20$      | $0$           |

![spinning_magnet_wave_plot](https://user-images.githubusercontent.com/7195133/227762226-2d7d6aca-262e-4e06-b00c-01dda2ec4ad7.jpg)  

In prima approssimazione, con i dati che abbiamo raccolto in tabella, si ha un onda triangolare. E' importante notare pero' che realisticamente, tracciando il flusso ad ogni istante nel tempo si avrebbe una sinusoide, come si vede in figura trattegiatta in arancione. In ogni caso il **valore medio** di questo tipo di onde e' **zero**, in quanto l'area sotto la curva nel quadrante positivo e' uguale all'area sotta la curva nel quadrante negativo.  

Conoscendo il comportamento del flusso nel tempo, possiamo allora derivare la tensione indotta nella spira grazie alla legge di Faraday-Neumann-Lenz e.g.    

$v_2 = \dfrac{\Delta \phi}{\Delta t} = \dfrac{\phi_2 - \phi_1}{t_2 - t_1} =\dfrac{1.6 - 0}{5 - 0} = \dfrac{1.6}{5} = 0.32\ V$  

#

| $index$ | $t\ [ms]$ | $\phi\ [mWb]$ | $v [V]$ |
| ------- | --------- | ------------- | ------- |
| $1$     | $0$       | $0$           | $0$     |
| $2$     | $5$       | $1.6$         | $0.32$  |
| $3$     | $10$      | $0$           | $-0.32$ |
| $4$     | $15$      | $-1.6$        | $-0.32$ |
| $5$     | $20$      | $0$           | $0.32$  |

![spinning_magnet_voltage_wave](https://user-images.githubusercontent.com/7195133/227763392-794c1c9e-d76e-4f47-9c46-4b63eb12d27e.jpg)  

