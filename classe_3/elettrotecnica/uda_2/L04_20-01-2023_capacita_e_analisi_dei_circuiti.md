# Capacita' di un condensatore  

L'equazione con cui abbiamo familiarizzato $C = \dfrac{Q}{V}$ potrebbe farci pensare che in qualche modo la capacita' dipende dalla tensione o dalla quantita' di carica, *sbagliato!*  
La capacita' e' una costante del condensatore e **dipende dalla sua geometria**.  

![capacitance_formula_geometry](https://user-images.githubusercontent.com/7195133/214650950-5f6b75aa-1d01-45ce-a0ba-356b5ec2fdb9.jpg)  

## Permittivita'  

Si puo' sperimentare che due condensatori uguali hanno capacita' diverse in dipendenza del loro dielettrico. Il dielettrico e' un qualunque mezzo nel quale possono verificarsi campi elettrostatici, quindi un mezzo **non conduttore** e.g. il vuoto, l'aria etc.  

E' stato sperimentato che la forza tra due cariche elettriche dipende non solo dalle cariche $Q_1, Q_2$ e dalla loro distanza $r^2$ ma anche dal mezzo in cui sono immerse.   

$F = k \dfrac{Q_1Q_2}{r^2}$  

La legge di *Coulomb* ci mostra appunto $k$, la *costante di Coulomb*, che puo' essere derivata conoscendo gli altri termini dell'equazione, e si presenta in questa forma:

$k = \dfrac{1}{4\pi\epsilon_0\epsilon_r}$  

La **costante dielettrica del vuoto** o anche *permittivita' del vuoto* e' $\epsilon_0$ ed ha un valore di circa:  

$\epsilon_0 = 8.8541 \cdot 10^{-12}\ F/m$  


Per convenzione si compara la permittivita' dei dielettrici rispetto a quella del vuoto, questa prende il nome di **permittivita' elettrica relativa**.  

$\epsilon_r = \dfrac{\epsilon}{\epsilon_0}$

E' una grandezza fisica che quantifica la propensione del materiale a contrastare l'intensita' di un campo elettrico presente al suo interno e.g. se $\epsilon_r = 2$ allora questo particolare dielettrico presentera' un opposizione al campo elettrico $2$ volte in piu' di quanto avverrebbe nel vuoto.  

## Capacita'  

Conoscendo il concetto di permittivita' possiamo allora esaminare la formula per il calcolo della capacita'.  

$C = \epsilon_r \epsilon_0 \dfrac{S}{d}$  

E' chiaro adesso che la capacita' dipende dalla superficie delle piastre, dalla distanza tra di esse, e ovviamente dal materiale del dielettrico.  

Dato che $\epsilon_r = \dfrac{\epsilon}{\epsilon_0} \implies \epsilon_r \epsilon_0 = \dfrac{\epsilon}{\epsilon_0} \epsilon_0$ allora possiamo semplicemente scrivere:  

$C = \epsilon \dfrac{S}{d}$