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

$V_{medio} = \dfrac{A_1^{\pm}+A_2^{\pm}+...+A_n^{\pm}}{t_{oss}}$  

Notiamo che esiste un pattern, percio' calcoliamo il valore medio soltanto per il periodo di ripetizione.  

$A^+ = \dfrac{50 \cdot 3}{2} = 75\ Vs$  

$A^- = -20 \cdot 7 = -140\ Vs$  

$V_{medio} = \dfrac{A^+ + A^-}{t_{oss}}= \dfrac{75 - 140}{10} = -6.5\ V$  

## ES. 4 Disegnare il grafico di una tensione sinusoidale avente le seguenti caratteristiche:  

- valore massimo 10 V
- periodo di ripetizione 20 ms
- valore 10 V all'istante 0

Intervallo di tempo di osservazione compreso tra 0 e 40 ms  

![fad_voltage_as_cosine](https://user-images.githubusercontent.com/7195133/236632116-bb36d26d-626c-48df-9ff1-63936daf4511.jpg)


# Esercizi facoltativi  
## Svolgi l'esercizio 1 con il "modello pratico"  

Questo modello considera il diodo come una resistenza $R_{Dx} = 30\ \Omega$ in serie ad un generatore di tensione $E_{Dx} = 0.6\ V$. I diodi pero' continuano ad essere interdetti, percio' nel circuito non c'e' corrente, e le tensioni sui diodi restano allora invariate.  

$V_{Dx} = E_{Dx} + R_{Dx}I_x = 0.6 + 30 \cdot 0 = 0.6\ V$  

$D1 = (-30\ V;\ 0\ A)$  
$D2 = (0\ V;\ 0\ A)$  

In questo caso il modello pratico non porta nessuna nuova informazione, non ci da' quindi nessun vantaggio rispetto al modello ideale.  

## Svolgi l'esercizio 2 con il "modello pratico"  

![fad_diodo_reale_fig2](https://user-images.githubusercontent.com/7195133/236646337-7b51894a-7316-4289-973b-dc254324b823.jpg)

Questo modello considera il diodo come una resistenza $R_{Dx} = 30\ \Omega$ in serie ad un generatore di tensione $E_{Dx} = 0.6\ V$. In questo scenario i diodi sono entrambi in conduzione, percio' per determinare i loro punti di lavoro possiamo utlizzare il metodo di Kirchhoff.  

$$
\begin{cases}
  \begin{aligned}
    I - I_1 - I_2 &= 0 \\
    E - E_{D1} - R_{D1}I - R_1I_1 &= 0 \\
    R_{D2}I_2 + E_{D2} + R_2I_2 - R_1I_1 &= 0 \\
  \end{aligned}
\end{cases}
$$

Sostituiamo $I_1$ alla seconda equazione.  

$I_1 = I - I_2$  
$E - E_{D1} - R_{D1}I - R_1(I - I_2) = 0$  
$E - E_{D1} - R_{D1}I - R_1I + R_1I_2 = 0$  

Sostituiamo $I_1$ alla terza equazione.  

$R_{D2}I_2 + E_{D2} + R_2I_2 - R_1(I - I_2) = 0$  
$R_{D2}I_2 + E_{D2} + R_2I_2 - R_1I + R_1I_2 = 0$  

Riscriviamo l'equazione sapendo che $R_1 = R_2 = 20\ k\Omega$ ed isoliamo $I_2$.  

$R_{D2}I_2 + E_{D2} - R_1I + 2R_1I_2 = 0$  

$I_2 = \dfrac{- E_{D2} +R_1I}{R_{D2} + 2R_1}$  

$I_2 = \dfrac{-0.6 + 20000I}{40030}$  

Sostiuiamo infine $I_2$ alla seconda equazione per isolare $I$.  

$E - E_{D1} - R_{D1}I - R_1I + R_1I_2 = 0$  

$E - E_{D1} - R_{D1}I - R_1I + R_1(\dfrac{-0.6 + 20000I}{40030}) = 0$  

$E - E_{D1} - R_{D1}I - R_1I + \dfrac{20000}{40030}(-0.6 + 20000I) = 0$  

$40 - 0.6 - 30I - 20000I -0.3 + 10000I = 0$  

$I = \dfrac{-40 +0.6 +0.3}{-10030} \simeq 3.89\ mA$  

Troviamo allora $I_2$ ed $I_1$.  

$I_2 = \dfrac{-0.6 + 20000I}{40030} = \dfrac{-0.6 + 20000 \cdot 0.00389}{40030} \simeq 1.9\ mA$  

$I_1 = I - I_2 = 3.89 - 1.9 = 1.99\ mA$  

Troviamo ora la tensione ai capi dei diodi:  

$V_{D1} = R_{D1}I + E_{D1} = 30 \cdot 0.00389 + 0.6 = 0.716\ V$  

$V_{D2} = R_{D2}I_2 + E_{D2} = 30 \cdot 0.0019 + 0.6 = 0.657\ V$  

Si ha allora che con il modello pratico i punti di lavoro dei diodi sono:  

$D1 = (0.716\ V;\ 3.89\ mA)$  
$D2 = (0.6\ V;\ 1.9\ mA)$  

I risultati non si discostano molto da quelli ottenuti con il modello ideale, ma si intuisce la maggiore accuratezza nel descrivere il sistema. Notiamo per esempio che $I_2 \ne I_1$ consenguenza del fatto che il diodo in conduzione non e' piu' considerato un cortocircuito.  
