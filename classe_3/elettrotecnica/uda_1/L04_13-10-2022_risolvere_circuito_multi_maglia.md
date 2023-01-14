# Risolvere un circuito multi maglia  

![circuito_multi_maglia_step_1](https://user-images.githubusercontent.com/7195133/197338653-2bdc8e6e-8237-4bb1-952b-0eaf0287021a.jpg)

Si prenda in considerazione un circuito con due maglie e 5 resistori come in firgura.  

$R_1 = 10\Omega$  
$R_2 = 15\Omega$  
$R_3 = 50\Omega$  
$R_4 = 25\Omega$  
$R_5 = 10\Omega$  

Per trovare la resistenza totale e' necessario semplificarlo, possiamo partire allora dalla maglia piu' esterna dove sappiamo che  
$R_2$ e $R_4$ sono in serie, e possiamo quindi calcolarne la resistenza equivalente utilizzando la formula dei resistori in serie $R_s = R_2 + R_4 = 40\Omega$  

![circuito_multi_maglia_step_2](https://user-images.githubusercontent.com/7195133/197338643-1b963e5c-8c0e-4e0a-9501-8663c11235b6.jpg)  

Questa semplificazione mette immediatamente in evidenza che $R_3$ ed $R_s$ sono in parallelo e possiamo allora utilizzare l'appropriata formula  
per calcolare la resistenza equivalente $R_p = \frac{R_3 \cdot R_s}{R_3 + R_s} = 22.\overline{2}\Omega$  

A questo punto siamo rimasti con $R_p$, $R_1$, ed $R_5$ in serie, quindi la resistenza totale del circuito e' $R_p + R_1 + R_5 = 22.\overline{2} + 10 + 10 = 42.\overline{2}\Omega$  

## Corto circuito
### Bypass del resistore

![extra_conducttore_nasconde_R5](https://user-images.githubusercontent.com/7195133/197339368-c127839e-c686-4a12-b2a5-4a727ecdc907.jpg)  

Aggiungendo un conduttore con resistenza idealmente nulla in parallelo a $R_5$ si ottiene un effetto *"bypass"* cioe' un corto circuito.  
La corrente allora scegliera' naturalmente la via con meno resistenza, ovvero la via che minimizza il consumo di energia, evitando quindi $R_5$.  
Realisiticamente pero' il conduttore non avra' mai resistenza nulla, e si avra' quindi, anche se trascurabile, un po' di corrente su $R_5$  
e di consequenza una (sempre trascurabile) caduta di potenziale. 
