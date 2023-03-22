# Protezioni da sovracorrenti  

Ricordiamo che esistono due sistuazioni in cui si presentano sovracorrenti, il **sovraccarico**, qundi una sovracorrente in un circuito elettricamente sano, ed il **cortocircuito**, ovvero una sovracorrente in un circuito guasto.  

Queste possono essere governate utilizzando due dispositivi di protezione, il fusibile ed il magnetotermico.  

## Magnetotermico  

![thermal_magnetic_curve](https://user-images.githubusercontent.com/7195133/227048673-d9ab364c-ff4b-4a12-9ea8-085c6213b8a0.jpg)  

In un impianto il magnetotermico deve soddisfare le seguenti condizioni:  

$I_b \le I_n \le I_z$  

$I_f \le 1.45 \cdot I_z$

* $I_b$ e' la corrente di impiego, ovvero la corrente che ci si aspetta in condizioni di funzionamento ordinarie
* $I_n$ e' invece la corrente nominale del dispositivo di protezione, ovvero quella corrente che il dispositivo di protezione puo' sopportare senza intervenire
* $I_f$ corrente di sicuro scatto, o anche detta di intervento del dispositivo di protezione 
* $I_z$ e' la portata del conduttore

La normativa di produzione prevede che la corrente di intervento dei magnetotermici soddisfi la seguente condizione:  

$I_f \le 1.45 \cdot I_n$  

Allora possiamo considerare nel peggiore dei casi $I_f = 1.45 \cdot I_n$ e possiamo quindi riscrivere la condizione di intervento come:    

$I_f \le 1.45 \cdot I_z \implies \cancel{1.45} \cdot I_n \le \cancel{1.45} \cdot I_z$  

Ne consegue che per i magnetotermici e' necessario soddisfare solo la condizione:  

$I_b \le I_n \le I_z$  

## Fusibile  

![fuse_curve](https://user-images.githubusercontent.com/7195133/227048731-d1a83f42-3b22-457b-9498-126f64c35fa7.jpg)

