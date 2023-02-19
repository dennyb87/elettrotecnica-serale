# Simulazione dimensionamento impianto  

Supponiamo di dover dimensionare l'impianto di un abitazione di area $120\ m^2$ con:  

* tensione nominale $230\ V_n$
* impianto luci di $1kW$ con $k_c = 0.8\ k_u = 1$  
* 10 prese da $10\ A$ con $k_p = 0.1$
* 3 prese da $16\ A$ con $k_p = 0.05$
* 1 boiler da $1.5\ kW$

![potenza_specifica_ambienti](https://user-images.githubusercontent.com/7195133/219973837-ea6f6ac0-90c2-47f2-8add-4b43e7c08edc.jpg)  

Per le abitazioni civili si stima $40\ VA/m^2$ allora supponendo un $cos \varphi = 0.9$ si stima una potenza attiva di circa:  

$P = 40 \cdot 120 \cdot 0.9 = 4320\ W$  

Andiamo a calcolare la potenza convenzionale, per avere un idea piu' precisa, e ovviamente la corrente di impiego.  

$P_{luci} = P \cdot k_c = 1000 \cdot 0.8 = 800\ W$  

$P_{prese10} = N \cdot V_n \cdot I_{max} \cdot \cos \varphi \cdot k_p = 10 \cdot 230 \cdot 10 \cdot 0.9 \cdot 0.1 = 2070\ W$  

$P_{prese16} = N \cdot V_n \cdot I_{max} \cdot \cos \varphi \cdot k_p = 3 \cdot 230 \cdot 16 \cdot 0.9 \cdot 0.05 = 496.8\ W$  

Calcoliamo ora la potenza convenzionale e la corrente di impiego considerano coefficienti di riduzione unitari per il boiler.  

$P_{c} = P_{luci} + P_{prese10} + P_{prese16} + P_{boiler} = 800 + 2070 + 496.8 + 1500 = 4866.8\ W$  

$I_b = \dfrac{P_{c}}{V_n \cdot \cos \varphi} = \dfrac{4866.8}{230 \cdot 0.9} \simeq 23.5\ A$  

## Sezione cavo  

Adesso vogliamo calcolare la sezione del cavo in **EPR** che va dal contatore al quadro generale supponendo la posa $4A$.  

![tpsee_posa_4-4A](https://user-images.githubusercontent.com/7195133/219974798-db2413d0-bd1f-4803-90ef-4bf16a5b6012.jpg)  

Sappiamo che la portata deve essere maggiore o uguale alla corrente di impiego $I_b \le I_z$ ovvero $23.5 \le I_z$. Troviamo la sezione sapendo che abbiamo a che fare con tre conduttori: fase, neutro, e protezione.  

![sezione_posa_a4](https://user-images.githubusercontent.com/7195133/219975398-f5568604-8d6a-4276-8d9a-329acd7c6068.jpg)![riduzione_posa_4a](https://user-images.githubusercontent.com/7195133/219975479-75a3c157-280a-456c-8606-76bd012e1b4e.jpg)  

Con 3 conduttori in **EPR** si ha allora una sezione di $4\ mm^2$ una portata $I_0 = 35\ A$ ed un coefficiente di riduzione per cavi installati a fascio $k_2 = 0.7$ considerando un $k_1$ unitario.  

$I_z = I_0 \cdot k_1 \cdot k_2 = 35 \cdot 0.7 = 24.5\ A$  

Un cavo di questo tipo soddisfa quindi la condizione $I_b \le I_z$ ovvero $23.5 \le 24.5$