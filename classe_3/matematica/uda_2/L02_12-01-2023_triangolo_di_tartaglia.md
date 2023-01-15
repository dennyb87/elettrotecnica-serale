# Triangolo di Tartaglia  

Se si provano a sviluppare i binomi in forma $(a + b)^n$ con $n \in \mathbb{N}$ ed $n \to \infty$ si nota immediatamente un pattern emergere nella distribuzione dei coefficienti.  

Vediamo infatti che coefficienti di $n + 1$ possono essere derivati dai coefficienti di $n$, e che il numero degli elementi di ogni riga del triangolo indica il numero di monomi necessari e.g. con $n = 2$ si ha una soluzione di $3$ monomi.  

![PascalTriangleAnimated2](https://user-images.githubusercontent.com/7195133/212536277-40b36511-2d44-41dc-b5d0-7b99abb743c1.gif)

Vediamo lo sviluppo con qualche valore di $n$

$(a + b)^2 = a^2 + 2ab + b^2$  
$(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$  
$(a + b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4$  
$...$  

E' importante notare che e' emerso un altro pattern dalle potenze delle parti letterali!  

$(a + b)^n = ka^{n-i_0}b^{i_0} + ...$  

Possiamo quindi risolvere in modo relativamente rapido qualunque potenza di binomio semplicemente sviluppando il risultato tenendo conto che i monomi assumono una forma $k_0a^{n-i_0}b^{i_0}$ dove i coefficienti $k$ vengono appunto dal *triangolo di Tartaglia*, mentre le potenze di $a$ diminuiscono all'aumentare dell'indice $i$ del monomio, e le potenze di $b$ crescono.  


# Notazione scientifica vs esponenziale  

Bisogna fare attenzione quando si parla di notazione scientifica in quanto e' definita come la riscrittura compatta di un numero come prodotto di un numero decimale da $1$ (incluso) a $10$ (escluso), e una potenza di $10$ con esponente intero.  

Differisce quindi da una semplice notazione esponenziale che non e' altro che un numero espresso come prodotto un numero qualunque e una potenza di $10$.

$1 \cdot 10^3 \implies\ notazione \ scientifica$  
$103 \cdot 10^3 \implies\ notazione \ esponenziale$  

A volte c'e' bisogno di trasformare due potenze con la stessa base per poterle sommare senza dover effettuare troppi calcoli, per esempio: 

$10^9 + 10^8$  

Se vogliamo evitare di dover calcolare le potenze, dobbiamo trovare un modo per trasformare l'espressione in modo da sommare due potenze uguali.  

$10^9 = 1 \cdot 10^9 = 1 \cdot 10 \cdot 10^8 = 10 \cdot 10^8$  

Adesso non ci resta che sommare i due monomi:  

$10^8 + 10 \cdot 10^8 = 1 \cdot 10^8 + 10 \cdot 10^8 = 11 \cdot 10^8$  

Alternativamente avremmo potuto traformare $10^8$  

$10^8 = 1 \cdot 10^8 = \dfrac{1}{10} \cdot 10^9 = 0.1 \cdot 10^9$  

$10^9 + 0.1 \cdot 10^9 = 1 \cdot 10^9 + 0.1 \cdot 10^9 = 1.1 \cdot 10^9$  

$11 \cdot 10^8 = 1.1 \cdot 10^9$  

Essenzialmente non stiamo altro che moltiplicando e dividendo per $10$ quindi il risultato non cambia!