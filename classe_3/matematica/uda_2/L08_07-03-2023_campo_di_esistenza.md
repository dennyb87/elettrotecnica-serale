# Campo di esistenza  

Si definisce **campo di esistenza** l'insieme dei valori attribuibili alle incognite per i quali e' possibile ottenere un risultato valutando l'espressione data. Prendiamo in considerazione la frazione algebrica:  

$\dfrac{a + b}{a^2 - b^2}$  

Per capire quale sia il campo di esistenza di questa frazione algebrica, bisogna capire in quali condizioni questa puo' esistere. Si nota immediatamente che l'unica condizione e' che il denominatore sia diverso da zero. Se fosse zero infatti il risultato potrebbe essere indeterminabile o impossibile.     

Adesso non ci resta che individuare quali siano i valori di $a$ e di $b$ per cui questa che rendono zero il denominatore. Per fare questo possiamo trovarli a occhio, oppure scomporre il denominatore semplificando la ricerca. Essendo una somma per differenza possiamo riscrivere il denominatore come:  

$\dfrac{a + b}{a^2 - b^2} = \dfrac{a + b}{(a + b)(a - b)}$  

Allora per la legge di annullamento del prodotto, il denominatore e' zero se almeno uno dei suoi fattori e' zero.  

$(a + b) = 0 \implies a = -b$  
$(a - b) = 0 \implies a = +b$  

Possiamo allora concludere che il campo di esistenza di questa frazione algebrica sia:  

$CE\ \ a \neq \pm b$  

Adesso e' importante notare cosa succede quando si semplificano i termini:  

$\dfrac{a + b}{a^2 - b^2} = \dfrac{\cancel{a + b}}{\cancel{(a + b)}(a - b)} = \dfrac{1}{a - b}$  

Si e' ottenuta quindi un'espressione $P_2$ che e' effetivamente equivalente all'espressione iniziale $P_1$ solo nel campo di esistenza di $P_1$ in quanto $\dfrac{1}{a - b}$ permette la condizione $a = -b$ ed ha quindi un campo di esistenza diverso da $P_1$.  

Questo diventa ancora piu' evidente se consideriamo la funzione:  

$f(x) = \dfrac{x^2 + 2x}{8x + 16} = \dfrac{x\ \cancel{(x + 2)}}{8\ \cancel{(x + 2)}} = \dfrac{x}{8}$  

Il campo di esistenza di $f(x)$ e' alllora $x \neq -2$ e condizione che renderebbe il denominatore zero, creando un **buco** nella curva della funzione, in quanto non esiste un valore di $y$ per la $x$ data come si nota in figura.  

![function_missing_value](https://user-images.githubusercontent.com/7195133/224515291-d749acde-aaa3-4e8e-b27e-64884520c4e9.jpg)  
