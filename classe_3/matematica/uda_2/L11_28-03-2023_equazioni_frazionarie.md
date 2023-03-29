# Equazioni frazionarie  

Si dice fratta o frazionaria un'equazione che presenta una frazione algebrica, ovvero un rapporto con l'incognita al denominatore, ad almeno uno dei suoi membri. Queste possono permettere una sola soluzione, infinite, o nessuna.  

## Equazione determinata $\implies$ una soluzione
$\dfrac{1}{x^2-4}-\dfrac{2}{x+2} = \dfrac{3}{x-2}$  

Scomponiamo i denominatori per trovare il campo di esistenza.  

$\dfrac{1}{(x+2)(x-2)}-\dfrac{2}{x+2} = \dfrac{3}{x-2}$  

$CE\ x \neq \pm 2$  

Poniamo ora l'equazione uguale a zero grazie alla regola del trasporto.  

$\dfrac{1}{(x+2)(x-2)}-\dfrac{2}{x+2} - \dfrac{3}{x-2} = 0$  

Trovato il denominatore comune possiamo allora sommare le frazioni.  

$\dfrac{1-2(x-2)-3(x+2)}{(x+2)(x-2)} = 0$  

$\dfrac{1-2x+4-3x-6}{(x+2)(x-2)} = 0$  

$\dfrac{-5x-1}{(x+2)(x-2)} = 0$  

Arrivati a questo punto vogliamo esaminare il primo membro e renderci conto che puo' essere uguale a zero solo quando il numeratore e' zero. Possiamo allora ignorare il denominatore dato che la sola condizione necessaria e' quella imposta dal campo di esistenza, in quanto qualunque denominatore non nullo, dara' come risultato zero se il numeratore e' zero.  

Procediamo allora ad esaminare quando il numeratore e' zero.  

$-5x-1 = 0$  

$-5x = 1$  

$\dfrac{\cancel{-5} \cdot x}{\cancel{-5}} = -\dfrac{1}{5}$  

Questa equazione allora permette una sola soluzione in quanto il numeratore e' zero soltanto quando $x = -\dfrac{1}{5}$ valore che soddisfa anche il campo di esistenza. Ogni altro valore di $x$ darebbe luogo ad un numeratore che e' diverso da zero, e percio' incompatibile con il secondo membro dell'equazione che e' appunto zero, oppure annullerebbe il denominatore rendendo la frazione impossibile.  

## Equazione indeterminata $\implies$ infinite soluzioni  

$\dfrac{1}{x^2-1}+\dfrac{1}{x^2-3x+2}=\dfrac{2x-1}{(x-2)(x^2-1)}$  

Scomponiamo i denominatori, utilizzando la formula per le equazioni di secondo grado per $x^2-3x+2$  

$x = \dfrac{-b \pm \sqrt{b^2 -4ac}}{2a} = \dfrac{3 \pm \sqrt{9 -8}}{2}$  

$x_1 = \dfrac{3+1}{2} = 2$  

$x_2 = \dfrac{3-1}{2} = 1$  

$x^2-3x+2 = (x-1)(x-2)$  

Procediamo allora alla scomposizione dei denominatori dell'equazione...  

$\dfrac{1}{(x+1)(x-1)}+\dfrac{1}{(x-1)(x-2)}-\dfrac{2x-1}{(x-2)(x+1)(x-1)} = 0$  

$\dfrac{x-2+x+1-(2x-1)}{(x-2)(x+1)(x-1)} = 0$  

$\dfrac{x-2+x+1-2x+1}{(x-2)(x+1)(x-1)} = 0$  

$\dfrac{0x+0}{(x-2)(x+1)(x-1)} = 0$  

Si nota allora che qualunque valore di $x$ che soddisfi il campo di esistenza annulla il denominatore, l'equazione permette allora infinite soluzioni ed e' percio' indeterminata.   


## Equazione impossibile $\implies$ non ammette soluzioni  

$\dfrac{1}{x^2-2x}-\dfrac{2}{x^2-4} = \dfrac{1}{x^2+2x}$  

$\dfrac{1}{x(x-2)}-\dfrac{2}{(x+2)(x-2)}-\dfrac{1}{(x+2)} = 0$  

$$
CE
\begin{cases}
    x \neq 0 \\
    x \neq \pm 2
\end{cases}
$$  

$\dfrac{(x+2)-2x-(x-2)}{x(x+2)(x-2)} = 0$  

$\dfrac{\cancel{x}+2-2x\ \cancel{-x}+2}{x(x+2)(x-2)} = 0$  

Troviamo allora che il numeratore e' zero quando...  

$-2x+4 = 0$  

$-2x = -4$  

$\dfrac{\cancel{-2} \cdot x}{\cancel{-2}} = \dfrac{-4}{-2} = 2$  

Scopriamo allora che l'unico valore di $x$ che annulla il numeratore, allo stesso tempo viola il campo di esistenza annullando il denominatore, l'equazione allora non permette soluzioni, ed e' quindi impossibile.  