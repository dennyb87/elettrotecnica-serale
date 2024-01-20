# Circuito resistivo in regime sinusoidale monofase  

![single_phase_resistive_circuit_schema](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/90d415a6-66d2-4d37-b562-48e0baeb9d0e)  

Si osservi lo schema di montaggio di un motore primo che aziona un generatore monofase alimentando un carico puramente resistivo. Prendendo in considerazione il circuito equivalente si vuole esaminare il comportamento delle grandezze elettriche in gioco.  

![simplified_single_phase_generator](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c5e78faf-3419-48cd-a47d-79fe3dedba31)  

In questa semplificazione di un generatore, possiamo osservare il **rotore**, in questo caso un magnete rotante, e lo **statore** su cui e' fissato un avvolgimento. La variazione di flusso nel tempo, dalla legge di *Faraday-Neumann-Lenz*, produce una tensione sinusoidale sull'avvolgimento come descritto in figura.  

E' dimostrabile che la tensione, cosi' come la frequenza, dipende dal numero di giri al minuto $n$ del rotore.  

$E_{max} = K_E \cdot n$  

$f = K_f \cdot n$  

Dove $K_E, K_f$ sono costanti che tengono conto di vari fattori come il numero di poli del generatore etc...  
Conoscendo il numero di giri e le relative costanti, possiamo allora ricavare la sinusoide delle grandezze in gioco nel circuito.  

$R = 10\ \Omega$  
$n = 3600\ \frac{giri}{min}$  
$K_E = 0.0333$  
$K_f = 0.0138$  

$E_{max} = K_E \cdot n = 0.0333 \cdot 3600 \simeq 120\ V$  

$f = K_f \cdot n \simeq 50\ Hz$  

$T = \dfrac{1}{f} = \dfrac{1}{50} = 0.02\ s = 20\ ms$  

$I_{max} = \dfrac{E_{max}}{R} = \dfrac{120}{10} = 12\ A$  

![single_phase_resistive_circuit_analysis](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/038117d8-a18b-4f05-a800-b8ea5865dbca)  
