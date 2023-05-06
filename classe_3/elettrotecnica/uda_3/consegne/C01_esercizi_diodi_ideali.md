# Esercizi sui diodi ideali  

## ES. 1 Determinare il punto lavoro dei diodi D1 e D2 nel circuito di Fig. 1  

![fad_diodi_ideali_fig1](https://user-images.githubusercontent.com/7195133/236326678-6f5e4a0c-a812-4e90-9e7f-616077812b81.jpg)  
![fad_diodi_ideali_eq_fig1](https://user-images.githubusercontent.com/7195133/236333191-a9175a9f-6e27-418e-a1f3-db664294254b.jpg)  

Troviamo il circuito equivalente consci del fatto che i diodi non sono in conduzione, percio' equivalgono a dei circuiti aperti (per comodita' rappresentati da interruttori utilizzando Multisim).  

Si ha allora grazie al secondo principio di Kirkhoff che:  

$V_{D1} = R_1 \cdot I_1 - E = 5000 \cdot 0 -30 = -30\ V$  
$V_{D2} = - R_1 \cdot I_1 + R_2 \cdot I_2 = - 5000 \cdot 0 + 10000 \cdot 0 = 0\ V$  

Percio' i punti di lavoro dei diodi sono rispettivamente:  

$D1 = (-30\ V;\ 0\ A)$  
$D2 = (0\ V;\ 0\ A)$  

## ES. 2 Determinare il punto lavoro dei diodi D1 e D2 nel circuito di Fig. 2  

![fad_diodi_ideali_fig2](https://user-images.githubusercontent.com/7195133/236328008-aed87f49-46f4-45b2-b0de-ca62c7003fbb.jpg)  

Invertendo il generatore si ha invece che entrambe i diodi sono in conduzione, quindi equivalenti ad un corto circuito.  

![fad_diodi_ideali_fig2](https://user-images.githubusercontent.com/7195133/236633569-6204d8d1-d82c-469d-8874-95280a87a558.jpg)

In questo caso essendo le resistenze in parallelo sappiamo che ai capi hanno la stessa tensione, quella del generatore, allora la corrente che attraversa $D2$ sara':  

$I_1 = I_2 = \dfrac{E}{R_2} = \dfrac{40}{20000} = 2\ mA$  

Allora la corrente $I$ che attraversa $D1$ sara':  

$I = I_1 + I_2 = 2I_2 = 2 \cdot 2 \cdot 10^{-3} = 4\ mA$  

I punti di lavoro dei diodi sono allora rispettivamente:  

$D1 = (0\ V;\ 4\ mA)$  
$D2 = (0\ V;\ 2\ mA)$  

## ES. 3 Calcolare il valore medio del segnale di Fig. 3  

![fad_diodi_ideali_fig3](https://user-images.githubusercontent.com/7195133/236328108-4e7c31a2-0993-4fe9-b425-51d1ece662c6.jpg)  

Sappiamo che il valore medio non e' altro che la somma algebrica delle aree descritte dalle curve nel tempo di osservazione, ovvero:  

$V_{medio} = \dfrac{A_1^{\pm}A_2^{\pm}+...+A_n^{\pm}}{t_{oss}}$  

Notiamo che esiste un pattern, percio' calcoliamo il valore medio soltanto per il periodo di ripetizione.  

$A^+ = 50 \cdot 3 = 150\ Vs$  

$A^- = -20 \cdot 7 = -140\ Vs$  

$V_{medio} = \dfrac{150 - 140}{10} = 1\ V$  

## ES. 4 Disegnare il grafico di una tensione sinusoidale avente le seguenti caratteristiche:  

- valore massimo 10 V
- periodo di ripetizione 20 ms
- valore 10 V all'istante 0

Intervallo di tempo di osservazione compreso tra 0 e 40 ms  

![fad_voltage_as_cosine](https://user-images.githubusercontent.com/7195133/236632116-bb36d26d-626c-48df-9ff1-63936daf4511.jpg)
