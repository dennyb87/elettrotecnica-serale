# Circuito capacitivo in onda triangolare  

![ac_triangular_capacitive_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1205f159-3b4c-4025-a817-0ab71e16066f)  

Si vuole esaminare il comportamento delle grandezze elettriche in un circuito puramente capacitivo alimentato da un generatore in alternata con onda triangolare. Si conoscono la capacita' del condensatore $C = 0.2\ F$ e i parametri fondamentali del generatore:  

* $E_{max} = 20\ V$
* $T = 2\ s$
* $\theta = 0^\circ$

Ricordando che e' possibile calcolare la quantita' di carica con $q = C \cdot V$ e' possibile tracciare le grandezze sul piano cartesiano accorgendosi che la tensione e  la carica sulle armature sono in fase.  

| $t\ [s]$ | $e(t)\ [V]$ | $q(t)\ [C]$ |
| -------- | ----------- | ----------- |
| 0        | 0           | 0           |
| 0.5      | 20          | 4           |
| 1        | 0           | 0           |
| 1.5      | -20         | -4          |
| 2        | 0           | 0           |

![emf_charge_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f32cdab5-862f-4228-b8e5-fd1b09de5ff5)  

Tracciamo infine anche l'andamento della corrente ricordando che $i(t) = \dfrac{\Delta q}{\Delta t}$ ovvero la pendenza di $q(t)$ ...  

| $t\ [s]$ | $\Delta q\ [C]$ | $\Delta t [s]$ | $i(t)\ [A]$ |
| -------- | --------------- | -------------- | ----------- |
| 0-0.5    | 4               | 0.5            | 8           |
| 0.5-1    | -4              | 0.5            | -8          |
| 1-1.5    | -4              | 0.5            | -8          |
| 1.5-2    | 4               | 0.5            | 8           |

![emf_charge_current_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ca8f8a49-2191-4d19-8832-e357fabb70e4)  

Approssimando $i(t)$ ad una sinusoide diventa evidente che la corrente in un circuito capacitivo e' in anticipo sulla tensione di $90^\circ$

![emf_charge_current_sine_approx](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b8e87219-2960-43de-aedb-2f30a3ab49a0)  
