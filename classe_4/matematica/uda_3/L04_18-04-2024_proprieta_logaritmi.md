# Proprieta' dei logaritmi  

## Definizione  

Si ricorda che...  

$a^c = b \implies \log_a b = c \implies a^{\log_a b} = b$  

Ne deriva anche che...  

$\log_a x = \log_a y \implies x = y$  

## Logaritmo del prodotto  

Dati due logaritmi con la stessa base possiamo derivare la regola del prodotto.  

$m = \log_a x \implies a^m = x$  
$n = \log_a y \implies a^n = y$  

Facendo il prodotto di entrambe i termini otteniamo...  

$a^ma^n = xy \implies a^{m+n} = xy$  

Quest'ultima espressione coincide con la definizione di logaritmo, per cui...  

$a^{m+n} = xy \implies \log_a xy = m+n$  

Sostituendo $m+n$ si ottiene infine...  

$\log_a xy = \log_a x + \log_a y$  

## Logaritmo del rapporto  

Riciclando le definizioni sopra possiamo scrivere:  

$\dfrac{a^m}{a^n} = \dfrac{x}{y} \implies a^{m-n} = \dfrac{x}{y}$  

$\log_a \bigg(\dfrac{x}{y}\bigg) = m-n$  

$\log_a \bigg(\dfrac{x}{y}\bigg) = \log_a m - \log_a n$  

## Regola dell'esponente  

$m = \log_a x \implies a^m = x$  

Aggiungiamo un'esponente in modo arbitrario...  

$(a^m)^n =  x^n \implies a^{mn} = x^n$  

Infine prendiamo il logaritmo in base $a$ per entrambe i membri...  

$\cancel{\log_a a}\ ^{mn} = \log_a x^n$  

Ma un logaritmo che ha come ha argomento la base si annulla e resta solo l'esponente, ovvero $\log_2 2^x = 1^x$ per cui...  

$mn = \log_a x^n$  

Infine sostituendo $mn$...  

$n \cdot \log_a x = \log_a x^n$  

## Formula del cambio di base  

$\log_a x = y$  

Dato questo logaritmo possiamo riscriverlo come rapporto tra due logaritmi in base $b$ vediamo come...  

$\log_a x = y \implies a^y = x$  

Prendendiamo il logaritmo in base $b$ per entrambe i membri...  

$\log_b a^y = \log_b x$

$y \cdot \log_b a = \log_b x$  

$y \cdot \cancel{\dfrac{\log_b a}{\log_b a}} = \dfrac{\log_b x}{\log_b a}$  

Sostiuiamo infine $y$...  

$\log_a x = \dfrac{\log_b x}{\log_b a}$  

## Logaritmo all'esponente  

$\log_a x = y \implies a^y = x$  

Sostituendo $y$ si ha allora che...  

$a^{\log_a x} = x$  

