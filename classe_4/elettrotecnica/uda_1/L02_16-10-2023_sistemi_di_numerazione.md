# Sistemi di numerazione  

Al contrario del sistema romano in cui ogni simbolo assume sempre lo stesso valore indipendentemente dalla sua posizione e.g $MDCCCLX = 1860$, il nostro sistema di numerazione, che anche il piu' usato, e' il **sitema decimale** ovvero un sistema di numerazione **posizionale** in **base 10**, dove qualunque numero puo' espresso come potenze di 10 utilizzando soltanto dieci simboli, le cifre da 0 a 9. Il peso di queste cifre dipende appunto dalla loro posizione, dove a destra si ha la meno significativa, mentre a sinistra quella piu' significativa.  

$1861 = 1 \cdot 10^3 + 8 \cdot 10^2 + 6 \cdot 10^1 + 1 \cdot 10^0$  

In modo analogo il **sistema binario** e' sempre un sistema di numerazione posizionale, ma in base 2, per cui i numeri vengono espressi come potenze di 2, utilizzando solo due simboli: $0$ ed $1$.  

$101_2 = 1 \cdot 2^2 + 0 \cdot 2^1 + 1 \cdot 2^0 = 5$  

# Conversioni  

Mentre la conversione da binario a decimale e' abbastanza intuitiva in quanto si tratta di una somma di potenze di 2 dove l'esponente e' la posizione della cifra su cui si effettua il prodotto:  

$1011_2 = 1 \cdot 2^3 + 0 \cdot 2^2 + 1 \cdot 2^1 + 1 \cdot 2^0 = 11$  

La conversione da decimale a binario sembra a prima vista misteriosa, ma in realta' stiamo effettuando la stessa operazione. Allora per trovare i *"blocchi"* che compongono il numero dobbiamo chiederci:  

* quanti $2^4$ servono ? 0 perche' e' maggiore di $11$
* quanti $2^3$ ? $1$
* quanti $2^2$ ? $0$
* quanti $2^1$ ? $1$
* quanti $2^0$ ? $1$

Il metodo meccanico consiste nel dividere ripetutamente per 2 fino a che non si arriva a zero.  

$$
\begin{aligned}
    11:2 &= 5\ resto\ 1\ LSD \\
    5:2  &= 2\ resto\ 1 \\
    2:2  &= 1\ resto\ 0 \\
    1:2  &= 0\ resto\ 1\ MSD \\
\end{aligned}
$$

Il resto di ogni divisione dipende dal fatto che il dividendo sia pari o dispari, per cui si ha che il significato del resto rappresenta il numero della potenza di 2 necessario in quella posizione e.g. quanti $2^0$ ?  

Il primo resto e' quindi il meno significativo, o *least significant digit* (LSD), in quanto rappresenta il numero $n$ di $2^0$ necessari, mentre l'ultimo e' il piu' significativo, *most significant digit* (MSD).  
