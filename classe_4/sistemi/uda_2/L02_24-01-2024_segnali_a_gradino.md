# Segnali a gradino  

![simple_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a590221c-12f1-48ef-bec3-67a5af8339c4)  

Per modellare la tensione nel tempo di un circuito semplice come in figura si ricorre all'uso della **funzione a gradino unitario**.  

$$
u(t) \coloneqq 
\begin{cases}
  \begin{aligned}
    0, \ \ t \lt 0 \\
    1, \ \ t \ge 0
  \end{aligned}
\end{cases}
$$

![funzione_gradino_unitaria](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/de1212d6-95a6-404a-9160-ba283e34621b)  

Se il circuito con un generatore da $E = 10\ V$ viene chiuso al tempo $t_s = 5$ si ha allora che la funzione $v(t)$ risulta essere...  

$v(t) = 10 \cdot u(t - 5)$  

In generale...  

$v(t) = E \cdot u(t - t_s)$  

![simple_circuit_step_function_model](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b4069bb3-3163-4056-b6d0-e5084ad67e32)  
