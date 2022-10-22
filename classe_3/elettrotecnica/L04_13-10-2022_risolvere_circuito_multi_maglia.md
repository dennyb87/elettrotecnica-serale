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
