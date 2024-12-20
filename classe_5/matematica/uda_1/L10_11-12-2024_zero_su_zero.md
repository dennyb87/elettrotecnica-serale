# Forma indeterminata zero su zero  

Puo' capitare che sostituendo il valore di tendenza nel calcolo di un limite si ottenga una forma indeterminata del tipo $\dfrac{0}{0}$  

$\displaystyle{\lim_{x\to 1}} \bigg(\dfrac{x^3-1}{x^2-1}\bigg) = \dfrac{1-1}{1-1} = \dfrac{0}{0}$  

Dato che qualunque numero moltiplicato per zero da come risultato zero, siamo di fronte ad una forma indeterminata. Ripartiamo dalla funzione originale espandendo la differenza di cubi al numeratore e la differenza di quadrati al denominatore...  

$(A^3-B^3) = (A-B)(A^2+AB+B^2)$  
$(A^2-B^2) = (A-B)(A+B)$  

$f(x) = \dfrac{x^3-1}{x^2-1} = \dfrac{\cancel{(x-1)}(x^2+x+1)}{\cancel{(x-1)}(x+1)}$  

$\displaystyle{\lim_{x\to 1}}\ f(x) = \dfrac{(x^2+x+1)}{(x+1)} = \dfrac{1+1+1}{1+1} = \dfrac{3}{2}$  

In sostanza, si manipola la funzione quanto possibile per eliminare il suo stato di indeterminazione.  
