# Esercizi
## Unita' 2 - Reti elettriche  
Pagina 360  

#
![elt_esercizio_12_pag_360](https://user-images.githubusercontent.com/7195133/202862914-78c2dc54-6b81-4370-bb90-4b92d4a9cfa0.jpg)  

In serie le resistenze sono attraversate dalla stessa corrente, che puo' essere  
quindi trovata con $I = \frac{E}{R_1 + R_2 + R_3 + R_4 + R_5} = \frac{24}{220 + 100 + 100 + 180 + 220} \simeq 0.0293A = 29.3mA$  

Adesso non ci resta che trovare le tensioni.  

$V_1 = R_1 \cdot I = 220 \cdot 0.0293 = 6.44V$  
$V_2 = R_2 \cdot I = 100 \cdot 0.0293 = 2.93V$  
$V_3 = R_3 \cdot I = 100 \cdot 0.0293 = 2.93V$  
$V_4 = R_4 \cdot I = 180 \cdot 0.0293 = 5.27V$  
$V_5 = R_5 \cdot I = 220 \cdot 0.0293 = 6.44V$  

$E = V_1 + V_2 + V_3 + V_4 + V_5 = 24V\ verificato\ \checkmark$

# 
![elt_esercizio_13_pag_360](https://user-images.githubusercontent.com/7195133/202862982-73d886c3-fcfd-4066-9ac0-60f5b7448266.jpg)  

Di nuovo essendo le resistenze in serie allora:

$I = \frac{V_2}{R_2} = \frac{3}{100} = 0.03A = 30mA$  
$R_{tot} = R_1+R_2+R_3+R_4+R_5 = 330 + 100 + 100 + 220 + 330 = 1080\Omega$  
$E = I \cdot R_{tot} = 0.03 \cdot 1080 = 32.4V$  

#
![elt_esercizio_14_pag_360](https://user-images.githubusercontent.com/7195133/202862990-2adc57ad-d06c-4add-9239-3abb5b851151.jpg)  

Se $R_4$ fa cadere $6V$ allora $R_1, R_2, R_3, R_5$ devono far cadere i restanti  
$6V$ in modo proporzionale alle loro resistenze.  

Troviamo quindi prima una delle tensioni:  
$V_1 = 6 \cdot \frac{R_1}{R_1 + R_2 + R_3 + R_5} = 6 \cdot \frac{1000}{1000 + 2000 + 680 + 560} = 1.415V$  

Per trovare la corrente ci basta $I = \frac{V_1}{R_1} = \frac{1.415}{1000} = 0.001415A$  
Adesso non dobbiamo far altro che trovare $R_4 = \frac{V_4}{I} = \frac{6}{0.001415} = 4240.28\Omega$  

Controlliamo che $V = I \cdot R_{tot}$  

$V = 0.001415 \cdot (4240.28 + 1000+ 2000 + 680 + 560) = 12V\ verificato\ \checkmark$ 


