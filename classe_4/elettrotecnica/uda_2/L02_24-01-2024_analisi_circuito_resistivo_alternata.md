# Analisi circuito resistivo in alternata  

Per determinare il comportamento delle grandezze in gioco in un circuito in regime alternato come in figura e' necessario conoscere la funzione che descrive l'andamento della tensione nel tempo, per cui si devono conoscere i **parametri fondamentali**:  

* ampiezza massima $A_{max}$
* periodo di ripetizione $T$
* fase $\theta$ ovvero l'angolo del vettore rotante all'istante $t = 0$

Si ricorda che una funzione sinusoidale puo' essere costruita partendo da un vettore rotante e viceversa.  

![sine_wave_phasor](https://user-images.githubusercontent.com/7195133/227787960-d96bb4a0-43a4-4765-88fd-fb5ddd7ba730.gif)  

Conoscendo allora i parametri fondamentali e' possibile derivare altre caratteristiche come:  

* ampiezza efficace $A = \dfrac{A_{max}}{\sqrt{2}}$
* ampiezza picco-picco $A_{pp} = 2A_{max}$
* frequenza di ripetizione $f = \dfrac{1}{T}$
* velocita' angolare del vettore rotante $\omega = 2\pi f$ oppure $\omega = 360^\circ f$ 

![simple_ac_resistive_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/55266992-3013-4dc9-8347-119d8c4094d8)  

Considerato il circuito resistivo in figura con $R = 4\  \Omega$ ed un generatore di tensione alternata, si vuole determinare il comportamento delle grandezze in gioco conoscendo i parametri fondamentali:

* $E_{max} = 20\ V$
* $T = 2\ s$
* $\theta = 0^\circ$

![simple_ac_circuit_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c878295f-7d6c-4db7-b379-e41d36daa410)  

$I_{max} = \dfrac{E_{max}}{R} = \dfrac{20}{4} = 5\ A$  

$P_{max} = E_{max} \cdot I_{max} = 20 \cdot 5 = 100\ W$  

Ricavando l'ampiezza massima della corrente $I_{max}$ e della potenza attiva $P_{max}$ e' possibile scrivere le loro funzioni in forma analitica e costruirne i grafici come in figura.  

$v(t) = E_{max} \cdot \sin \bigg(\omega \cdot t + \theta \bigg) = 20 \cdot \sin \bigg(\dfrac{2\pi}{2} \cdot t + 0\bigg) = 20 \cdot \sin (\pi \cdot t)$  

$i(t) = I_{max} \cdot \sin \bigg(\omega \cdot t+ \theta \bigg) = 5 \cdot \sin (\pi \cdot t)$  

$p(t) = v(t) \cdot i(t) = 20 \cdot \sin (\pi \cdot t) \cdot 5 \cdot \sin (\pi \cdot t) = 100 \cdot \sin (\pi \cdot t)^2$  

Troviamo infine i valori efficaci di tensione e corrente, e la potenza media.  

$E_{eff} = \dfrac{E_{max}}{\sqrt{2}} = \dfrac{20}{\sqrt{2}} \simeq 14.14\ V$  

$I_{eff} = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{5}{\sqrt{2}} \simeq 3.55\ A$  

$P_{avg} = \dfrac{E_{max}}{\sqrt{2}} \cdot \dfrac{I_{max}}{\sqrt{2}} = \dfrac{E_{max} \cdot I_{max}}{2} = \dfrac{20 \cdot 5}{2} = 50\ W$  

![valori_efficaci_e_potenza_media](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/4eaab6cb-b8ae-40d1-814b-1af51f806965)  
