# Partitore di tensione  

![voltage_divider](https://user-images.githubusercontent.com/7195133/206300542-a598b6ec-64ab-4286-a986-32d201726c78.jpg)

Abbiamo gia' affrontanto l'argomento in sistemi, ricordiamo quindi le formule per calcolare   
la tensione in uscita, che come e' ormai noto e' proporzionale al rapporto tra $R$ e $R_{tot}$.  

$V_{1} = \frac{R_1}{R_1 + R_2} \cdot V = R_1 \cdot I$  
$V_{2} = \frac{R_2}{R_1 + R_2} \cdot V = R_2 \cdot I$  

Nel caso speciale in cui $R_1 = R_2$ allora possiamo risolvere con una singola $R$  
trovando che la tensione e' di conseguenza sempre la meta'.

$V_{2} = \frac{R}{R + R} \cdot V = \frac{R}{2 \cdot R} \cdot V = \frac{1}{2} \cdot V$  


# Partitore di corrente  

Il partitore di corrente funziona in modo analogo: la corrente di un ramo e' proporzionale  
al rapporto tra la resistenza sul ramo adiacente e la somma delle resistenze nella maglia.  

![current_divider](https://user-images.githubusercontent.com/7195133/206303085-030a721a-70d3-4ece-9147-04c5e3dee3c7.jpg)  

$I_1 = \frac{R_2}{R_1 + R_2} \cdot I$  
$I_2 = \frac{R_1}{R_1 + R_2} \cdot I$  

Il motivo per cui questo e' vero e funziona e' tutt'altro che ovvio, ci serve allora  
una dimostrazione...  


# Dimostrazione del partitore di corrente  

![dimostrazione_partitore_di_corrente](https://user-images.githubusercontent.com/7195133/206860760-fa2493c6-a119-49d7-aad9-45591e03dafd.jpg)


Conoscendo la legge di Ohm $V_{ab} = I \cdot R_{p}$ e la formula per il calcolo delle  
resistenze in parallelo $R_{p} = \frac{R_1 \cdot R_2}{R_1 + R_2}$ possiamo allora derivare il partitore di  
corrente, e quindi dimostrare che e' vero!  

$I_1 = \frac{V_{ab}}{R_1}$  
$V_{ab} = I \cdot R_{p} = I \cdot \frac{R_1 \cdot R_2}{R_1 + R_2}$  
$I_1 = I \cdot \frac{R_1 \cdot R_2}{R_1 + R_2} \cdot \frac{1}{R_1} = I \cdot \frac{R_2}{R_1 + R_2}$  