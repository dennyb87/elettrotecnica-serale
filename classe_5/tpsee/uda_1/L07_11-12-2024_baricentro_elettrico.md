# Baricentro elettrico  

Il metodo del baricentro elettrico ci permette di posizionare quadri, cabine o qualunque centro di smistamento, nel punto geografico che **minimizza le perdite**. Si consideri la situazione seguente dove si hanno tre capannoni industriali distribuiti su un terreno come in figura.  

![baricentro_elettrico](https://github.com/user-attachments/assets/a2353bf0-d3be-4142-86ac-b49a815e2931)    

$P_1 = 100\ kW$  
$P_2 = 300\ kW$  
$P_3 = 400\ kW$  

Questo metodo consiste nell'individuare le coordinate nel piano cartesiano dei punti dove l'energia viene consumata. Per semplicita' si ipotizza che questi punti siano al centro dei capannoni.  

$P_1 = (20,\ 15)$  
$P_2 = (30,\ 105)$  
$P_3 = (170,\ 65)$  

Una volta trovati i punti, si calcola la media ponderata che restituisce il punto con le minime perdite, ovvero il baricentro elettrico $B_E$  

$X_{B_E} = \dfrac{P_1x_1+P_2x_2+P_3x_3}{P_1+P_2+P_3} = \dfrac{100\cdot 20+300\cdot 30+400\cdot 170}{100+300+400} = 98.75\ m$  

$Y_{B_E} = \dfrac{P_1y_1+P_2y_2+P_3y_3}{P_1+P_2+P_3} = \dfrac{100\cdot 15+300\cdot 105+400\cdot 65}{100+300+400} = 73.75\ m$  

$B_{E} = (X_{B_E},\ Y_{B_E}) = (98.75,\ 73.75)$  
