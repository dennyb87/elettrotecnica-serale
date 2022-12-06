# Calcolo del valore medio di un segnale    

Se si traccia l'andamento di un valore che varia nel tempo si puo' ottenere un  
grafico di questo tipo, con il tempo sull'asse delle $x$ e il valore sull'asse delle $y$

![grafici_e_segnali_fig1](https://user-images.githubusercontent.com/7195133/206029691-ed101a95-1616-4f6e-9633-443231c3503e.jpg)  

Si nota immediatamente che l'area sotto la curva puo' essere vista come un insieme  
di rettangoli e triangoli, oppure rettangoli e trapezi.  
In entrambe i casi si puo' calcolare l'area totale sotto la curva semplicemente  
sommando appunto le aree dei poligoni sotto la curva stessa, nel nostro caso  
rettangoli $A_{r1}, A_{r2}$ e dei trapezi $A_{t1}, A_{t2}$  

Ricordiamo la formula per il calcolo dell'area di un rettangolo $A_r = a \cdot b$  
e la formula per l'area di un trapezio $A_t = \frac{(a + b) \cdot h}{2}$  

$A_{r1} = 4 \cdot 8 = 32$  
$A_{r2} = 4 \cdot 12 = 48$  
$A_{t1} = \frac{(4 + 12) \cdot 4}{2} = 32$  
$A_{t2} = \frac{(2 + 12) \cdot 8}{2} = 56$  

Troviamo quindi l'area totale:  

$A = A_{r1} + A_{r2} + A_{t1} + A_{t2} = 32 + 48 + 32 + 56 = 168$  

Adesso per trovare il valore medio non ci resta che dividere l'area per il tempo di osservazione.  

$V_{medio} = \frac{Area}{T_{oss}} = \frac{A}{\Delta t} = \frac{168}{24} = 7$  


# Esempio con valore negativo  
...

# Calcolo velocita' di variazione  
...