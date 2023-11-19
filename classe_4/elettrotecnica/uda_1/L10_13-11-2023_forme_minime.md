# Forme minime  

Una funzione logica e' detta in **forma minima** quando non e' piu' semplificabile. Questa comporta notevoli vantaggi come: circuito piu' semplice, minore ingombro, costi ridotti, e maggiore affidabilita'.  

Da una tabella di verita' e' possibile ricavare la funzione logica ad esempio considerando esplicitando quando gli output sono uguali a 1.  

| A   | B   | Y   |
| --- | --- | --- |
| 0   | 0   | 0   |
| 0   | 1   | 1   |
| 1   | 0   | 1   |
| 1   | 1   | 0   |

Nel caso di una porta **XOR** allora si ha che l'uscita e' 1 quando gli ingressi sono diversi tra loro, per cui:  

$Y = \overline{A} \cdot B + A \cdot \overline{B}$  

In questo caso siamo davanti ad una forma minima in quanto non e' ulteriormente semplificabile. Con una tabella piu' complessa saremmo invece costretti a ridurre la funzione alla sua forma minima utilizzando le proprieta' dell'algebra booleana.  

| A   | B   | C   | Y   |
| --- | --- | --- | --- |
| 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 0   |
| 0   | 1   | 0   | 1   |
| 0   | 1   | 1   | 1   |
| ... | ... | ... | ... |

$Y = \overline{A}B\overline{C}+\overline{A}BC+...$  

