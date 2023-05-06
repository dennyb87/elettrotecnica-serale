# Esercizi sui diodi ideali  

## ES. 1 Determinare il punto lavoro dei diodi D1 e D2 nel circuito di Fig. 1  

![fad_diodi_ideali_fig1](https://user-images.githubusercontent.com/7195133/236326678-6f5e4a0c-a812-4e90-9e7f-616077812b81.jpg)  
![fad_diodi_ideali_eq_fig1](https://user-images.githubusercontent.com/7195133/236333191-a9175a9f-6e27-418e-a1f3-db664294254b.jpg)  

Troviamo il circuito equivalente consci del fatto che i diodi non sono in conduzione, percio' equivalgono a dei circuiti aperti (per comodita' rappresentati da interruttori utilizzando Multisim).  

Si ha allora che:  

$V_{D1} = R_1 \cdot I_1 - E = 5000 \cdot 0 -30 = -30\ V$  
$V_{D2} = - R_1 \cdot I_1 + R_2 \cdot I_2 = - 5000 \cdot 0 + 10000 \cdot 0 = 0\ V$  

Percio' i punti di lavoro dei diodi sono rispettivamente:  

$D1 = (-30\ V;\ 0\ A)$  
$D2 = (0\ V;\ 0\ A)$  

## ES. 2 Determinare il punto lavoro dei diodi D1 e D2 nel circuito di Fig. 2  

![fad_diodi_ideali_fig2](https://user-images.githubusercontent.com/7195133/236328008-aed87f49-46f4-45b2-b0de-ca62c7003fbb.jpg)  

Invertendo il generatore si ha invece che entrambe i diodi sono in conduzione, quindi equivalenti ad un corto circuito.  

![fad_diodi_ideali_eq_fig2](https://user-images.githubusercontent.com/7195133/236611683-3600f61e-55f3-471c-9676-f10f4e7f2f45.jpg)  

In questo caso essendo le resistenze in parallelo sappiamo che ai capi hanno la stessa tensione, quella del generatore, allora la corrente che attraversa $D2$ sara':  

$I_2 = \dfrac{E}{R_2} = \dfrac{30}{10000} = 3\ mA$  

Mentre la corrente $I_1$ che attraversa $R_1$ sara':  

$I_1 = \dfrac{E}{R_1} = \dfrac{30}{5000} = 6\ mA$  

Allora la corrente $I$ che attraversa $D1$ sara':  

$I = I_1 + I_2 = 3 \cdot 10^{-3} + 6 \cdot 10^{-3} = 9\ mA$  

I punti di lavoro dei diodi sono allora rispettivamente:  

$D1 = (0\ V;\ 9\ mA)$  
$D2 = (0\ V;\ 3\ mA)$  

## ES. 3 Calcolare il valore medio del segnale di Fig. 3  

![fad_diodi_ideali_fig3](https://user-images.githubusercontent.com/7195133/236328108-4e7c31a2-0993-4fe9-b425-51d1ece662c6.jpg)  


## ES. 4 Disegnare il grafico di una tensione sinusoidale avente le seguenti caratteristiche:  

- valore massimo 10 V
- periodo di ripetizione 20 ms
- valore 10 V all'istante 0

Intervallo di tempo di osservazione compreso tra 0 e 40 ms