# Divisione tra polinomi  

## Solo tra monomi simili  

Prendiamo in esame una semplice divisione tra monomi simili:  

$2a^2 : a$  

Pur non conoscendo il valore di $a$ possiamo immediatamente risolverla.  

$2a^2 : a = \dfrac{2 \cdot a \cdot a}{a} = 2a$  

Vediamo cosa succede quando i monomi **non sono simili**:  

$2a^2 : b$  

Va da se' che senza conoscere i valori di $a$ e di $b$ non e' possibile procedere oltre dato che non c'e' modo di sapere se, e quante volte $b$ sta' in $2a^2$.  
Per questo motivo la divisione tra polinomi con monomi non simili non e' possibile.  

## Grado e divisibilita'

La definizione di divisione tra polinomi e' identica a quella dei numeri naturali.  

> Dati due polinomi $A$ e $B$ esistono due polinomi **unici** $Q$ ed $R$ tali che:  
> $A = Q \cdot B + R$

E' importante precisare che il divisore $B$ deve avere grado minore o uguale al grado del dividendo $A$. Se cosi' non fosse la frazione sarebbe **propria** dando vita ad un $Q$ con esponente negativo, cessando quindi di essere un polinomio, che per definizione e' una somma algebrica di monomi, i quali sempre per definizione devono avere grado maggiore o uguale a zero.  

$a^2 : a^3 = a^{-1} = \dfrac{1}{a}$  

## Divisibilita' con o senza resto  

Un polinomio e' divisibile per un monomio (non nullo) e senza resto, solo se lo sono tutti i suoi termini e.g. $a^3 + 2a$ e' divisibile per $3a$, mentre $a^3 + 2a + 1$ non e' divisibile per $3a$ almeno non senza resto.  

$a^3 + 2a = \dfrac{a^2 + 2}{3} \cdot 3a$  

$a^3 + 2a + 1 = \dfrac{a^2 + 2}{3} \cdot 3a + 1$  

Risolvendo la seconda si ottiene in effetti un resto di $1$.

# Esempio con resto  

$(-3x^2 + 4 + 2x^4) : (x^2 - 4)$  

La divisione tra polinomi sfrutta lo stesso sistema della classica divisione numerica.  
Per fare leva sulla numerazione posizionale si devono prima di tutto ordinare i monomi per grado da sinistra verso destra.  

$(2x^4 -3x^2 + 4) : (x^2 - 4)$  

Possiamo ora procedere come una normale divisione numerica dividendo pero' i termini di grado massimo al numeratore con quelli di grado massimo del denominatore e.g. $2x^4 : x^2$  e moltiplicando il quoziente per il divisore $2x^2 \cdot (x^2 - 4)$ come in figura (in rosso).  

![polynomial_division_example_01](https://user-images.githubusercontent.com/7195133/213918993-af2fdf72-701f-43c5-8226-1252679fc0be.jpg)

Si puo' ripete la procedura a patto che il grado del divisore sia maggiore o uguale a grado del resto, nel momento in cui questa condizione smette di verificarsi si deve necessariamente interrompere l'esecuzione in quanto abbiamo trovato il resto.  

In questo caso e' $2x^2 + 5$ e' il quoziente mentre $24$ e' il resto.  

# Interpretazione geometrica  

Si prenda in considerazione la seguente divisione:  

$(a^2 + a) : (a^2 + 1)$  

Per definizione deve esistere un polinomio $Q(a)$ tale che $(a^2 + a) = Q(a) \cdot (a^2 + 1) + R$  
Prendiamo come esempio per semplicita' $a = 2$  

$(a^2 + a) : (a^2 + 1) = (2^2 + 2) : (2^2 + 1) = (4 + 2) : (4 + 1) = 6 : 5$  

Geometricamente significa trovare il lato mancante di un'area, quel lato che moltiplicato per $4 + 1$ dia come risultato $6$. In questo caso non esiste un lato in $\mathbb{N}$ percio' si avra' un resto ovviamente di $1$.  

![poly_division_geometric_interpretation](https://user-images.githubusercontent.com/7195133/213932049-4899ab98-5350-4813-a8e1-e1bd4a9a3676.jpg)  

Per arrivare a questo risultato senza conoscere il valore dell'incognita $a$ si procede come accennato sopra facendo attenzione a ad inserire i termini mancanti con coefficienti nulli.

$$
\begin{aligned}
a^2 + a + 0\ &|\ a^2 + 1 \\
{------}&|{---}\\
{-} a^2 -0a - 1\ &|\ 1 \\
{------}&|\\
a - 1\ &|
\end{aligned}
$$

Si ha allora che il quoziente e' uguale a $1$ mentre il resto e' $a - 1$.  
Se poniamo $a = 2$ si ha che:  

$(a^2 + a) = (a^2 + 1) \cdot 1 + a - 1$  

$2^2 + 2 = (2^2 + 1) \cdot 1 + 2 - 1$  

$6 = (4 + 1) \cdot 1 + 2 - 1$  

## Moltiplicazione del quoziente  

La moltiplicazione del quoziente (talvolta parziale) per il divisore ad ogni passaggio puo' apparire poco chiaro ma proviamo a spiegare perche' e' necessario. Ad ogni passaggio si divide il termine di grado massimo del dividendo per il termine di grado massimo del divisore. Questo ci permette di trovare un quoziente che se moltiplicato per il divisore dara' un risultato minore o uguale al dividendo.    

Quando il risultato della moltiplicazione e' minore del dividendo, significa che 


# Metodo di Ruffini  

Il metodo di *Ruffini* ci permette di dividere rapidamente un polinomio qualunque, per un binomio di primo grado della forma $x - r$. Questo tipo di divisione e' anche noto come *divisione sintetica* (*synthetic division* in inglese).  

Prendiamo in considerazione la seguente divisione:

$(x^3 - 2x^2 + 5x - 6) : (x - 3)$

Si scrive nella colonna di sinistra quel numero $r$ che rende il polinomio al denominatore uguale a zero, ovvero $3$ dato che $x - 3 = 3 - 3 = 0$. Cominciamo ora a sommare i coefficienti verticalmente da sinistra verso destra, si moltiplica il risultato per $r$ quindi per $3$ in questo caso, e cosi' via. I coefficienti fino a $c_{n-1}$ fanno parte del quoziente, mentre l'ultimo e' il resto, che non puo' avere parte letterale visto che al denominatore si ha un polinomio di primo grado.  

![ruffini_rule](https://user-images.githubusercontent.com/7195133/214431854-80dde106-0bad-4241-8c52-81b8e30a7408.jpg)  

Il procedimento fa leva sul fatto che il divisore sia di primo grado, permettendo una risoluzione piu' rapida grazie alla manipolazione dei soli coefficienti, ma essenzialmente sono gli stessi passaggi della classica divisione tra polinomi.  


## Ruffini e la proprieta' invariantiva  

$(2x^3 - 3x -1) : (2x -1)$  

Si puo' utilizzare Ruffini anche quando i coefficienti della parte letterale al denominatore sono maggiori di $1$. Questo e' possibile applicando la proprieta' invariantiva.  

$(2x^3 - 3x -1) : (2x -1) = \dfrac{(2x^3 - 3x -1)}{2} : \dfrac{(2x -1)}{2} = (x^3 - \frac{3}{2}x -1) : (x - \frac{1}{2})$  

Bisogna solo tenere a mente che pur ottenendo lo stesso quoziente, il resto dovra' necessariamente essere riportato alla forma originale con una trasformazione inversa ovvero, moltiplicato per $2$ in questo caso, visto che inizialmente abbiamo diviso entrambe i termini per $2$.  

# Coefficienti letterali  

Facciamo presente che e' possibile trattare coefficienti in forma letterale esattamente nello stesso modo con cui trattiamo i coefficienti numerici e.g.  

$(ax^4 - 3x^3 -x -a) : (x^2 + 1)$  

Il coefficiente letterale in questo caso e' $a$ e la divisione si svolge esattamente nello stesso modo ottenendo:  

$Q = ax^2 - 3x - a$    
$R = 2x$  