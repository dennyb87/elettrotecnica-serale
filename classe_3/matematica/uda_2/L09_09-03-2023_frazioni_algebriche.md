# Frazioni algebriche  

Nel momento in cui si ha un incognita al denominatore stiamo parlando di una **frazione algebrica**, ovvero un **rapporto tra polinomi** e.g. $\dfrac{2x + 8}{x}$  
Potremmo scrivere $(2x + 8) \cdot x^{-1}$ ma per *definzione* stiamo comunque parlando di una frazione algebrica e non di un semplice polinomio.  

Prendiamo in considerazione la seguente espressione:  

$\dfrac{1}{a^2-2a+1} + \dfrac{7}{2a-2} + \dfrac{1}{2a+2}$  

Per trasformarla in una frazione algebrica, quindi in un rapporto tra polinomi, bisogna trovare il denominatore comune in modo analogo quello per le frazioni numeriche:  

1. scomposizione denominatori
2. $m.c.m.$ tra denominatori
3. campo di esistenza

## Scomposizione  

$\dfrac{1}{a^2-2a+1} + \dfrac{7}{2a-2} + \dfrac{1}{2a+2}$  

Si vede immediatamente che il primo denominatore $D_1$ e' un quadrato di binomio, mentre per i restanti si puo' raccogliere la $a$.  

$D_1 = a^2 - 2a + 1 = (a - 1)^2$  
$D_2 = 2a - 2 = 2(a - 1)$  
$D_3 = 2a - 2 = 2(a + 1)$  

## Denominatore comune  

Il minimo comune multiplo e' quindi il prodotto tra i fattori comuni e non comuni con esponente maggiore, ovvero:  

$2(a+1)(a - 1)^2$  

## Campo di esistenza  

Una volta trovato il denominatore comune possiamo allora esaminare quali siano le condizioni di esistenza di questa frazione algebrica.  

$2(a+1)(a - 1)^2$  

In questo caso possiamo concludere che i valori di $a$ che annullano il denominatore sono $a \pm 1$  

$CE
\begin{cases}
    a \pm 1
\end{cases}$  

## Frazione algebrica  

Una volta trovato il denominatore comune possiamo procedere in modo analogo ad una somma di frazioni numeriche, trasformando i numeratori e sommandoli.  

$\dfrac{2(a+1) + 7(a + 1)(a - 1) + (a - 1)^2}{2(a+1)(a - 1)^2}$  

$\dfrac{2a + 2 + 7(a^2 - 1) + a^2 - 2a + 1}{2(a+1)(a - 1)^2}$  

$\dfrac{\cancel{2a} + 2 + 7a^2 - 7 + a^2 \cancel{- 2a} + 1}{2(a+1)(a - 1)^2}$  

$\dfrac{8a^2 - 4}{2(a+1)(a - 1)^2}$  

$\dfrac{\cancel{2}\cdot 2(2a^2 - 1)}{\cancel{2}(a+1)(a - 1)^2}$  