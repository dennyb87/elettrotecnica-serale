# Simulazione dimensionamento impianto  

Vogliamo calcolare il carico convenzionale, quindi la potenza convenzionale e la corrente di impiego, di un impianto formato da:

* 2 motori ognuno con potenza nominale di $3\ kW$ e rendimento $0.9$
* 2 gruppi di 3 prese $10/16A$  

Cominciamo dai motori identificando la potenza assorbita $P_{a}$  

$P_a = \dfrac{P_n}{\eta} = \dfrac{3000}{0.9} \simeq 3333.33\ kW$  

Possiamo ora calcolare la **potenza convenzionale  dei motori** con $N$ uguale al numero dei motori, e $K_u,K_c$ forniti da un'opportuna tabella di coefficienti.   

$P_{c1} = N \cdot P_a \cdot K_u \cdot K_c = 2 \cdot 3333.33 \cdot 0.75 \cdot 0.7 = 3500\ W$  

Passiamo al calcolo dei gruppi prese, dove $N$ e' ancora il numero di prese, e i coefficienti sono stavolta espressi come singolo coefficiente di riduzione $K_p = 0.1$ mentre $\cos \varphi$ si stima essere uguale a $0.9$  
Sappiamo invece che la tensione nominale e' ovviamente $230\ V$ mentre la corrente massima delle prese e' di $16\ A$  

$P_{c2} = N \cdot V_n \cdot I_n \cdot \cos \varphi \cdot K_p = 6 \cdot 230 \cdot 16 \cdot 0.9 \cdot 0.1 = 1987.2\ W$  

Troviamo allora la potenza convenzionale totale: 

$P_{tot} = P_{c1} + P_{c2} = 3500 + 1987.2 = 5487.2\ W$  

La corrente di impiego sara' quindi:  

$I_b = \dfrac{P_{tot}}{V_n \cdot \cos \varphi} = \dfrac{5487.2}{230 \cdot 0.9} \simeq 26.5\ A$  
