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

$(a^4 + a^3) : (a^2 + 1)$  

Per definizione deve esistere un polinomio $Q(a)$ tale che $(a^4 + a^3) = Q(a) \cdot (a^2 + 1) + R$  
Prendiamo come esempio per semplicita' $a = 2$  

$(a^4 + a^3) : (a^2 + 1) = (2^4 + 2^3) : (2^2 + 1) = (16 + 8) : (4 + 1) = 24 : 5$  

Geometricamente significa trovare il lato mancante di un'area, quel lato che moltiplicato per $4 + 1$ dia come risultato $24$.  

![polynomial_division_geometric_interpretation](https://user-images.githubusercontent.com/7195133/213922281-c610e39e-c446-46a3-ad50-b4e42bbebb3e.jpg)
