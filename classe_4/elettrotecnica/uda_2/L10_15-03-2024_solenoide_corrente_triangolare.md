# Solenoide in corrente triangolare  

![sine_current_solenoid_1](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/89dd9401-a242-4ba9-abff-7fee7ae90cbb)  

Si consideri un solenoide con avvolgimento su ferro tale che la sua induttanza risulta $L = 32\ mH$. La corrente con cui e' alimentato il solenoide e' alternata con forma d'onda triangolare, valore medio nullo, valore massimo $2\ A$, periodo di ripetizione $4\ s$.  

Possiamo allora tracciare la corrente e il flusso concatenato $\phi_c$ sapendo che $\phi_c = L \cdot I$  

${\phi_c}_{max} = L \cdot I_{max} = 32 \cdot 10^{-3} \cdot 2 = 64\ mWb = 0.64\ dWb$  

![sine_current_solenoid_2](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/20447b1a-a197-4112-826d-be4436bdb547)  

Per trovare infine la tensione indotta sul solenoide si ricorre invece alla legge di *Faraday-Neumann-Lenz* $v = \dfrac{\Delta \phi}{\Delta t}$  

| $intervallo\ [s]$ | $\Delta \phi\ [dWb]$ | $\Delta t\ [s]$ | $v\ [dV]$ |
| ----------------- | -------------------- | --------------- | --------- |
| $0 \div 1$        | $0.64$               | $1$             | $0.64$    |
| $1 \div 2$        | $-0.64$              | $1$             | $-0.64$   |
| $2 \div 3$        | $-0.64$              | $1$             | $-0.64$   |
| $3 \div 4$        | $0.64$               | $1$             | $0.64$    |

![sine_current_solenoid_3](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/8f310c54-e7db-474e-add0-2cadaf88d21b)  

Approssimando la tensione a una sinusoide diventa evidente come, al contrario di un circuito capacitivo, la corrente sia in ritardo di $90^\circ$ rispetto alla tensione.  

![sine_current_solenoid_4](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/47d74daa-a8c6-4599-8da8-a52065d798ca)  

Tracciando infine la potenza si puo' notare non solo che ha valore medio nullo, ma anche che ha il doppio della frequenza delle altre grandezze.  

$P_{max} = V_{max} \cdot V_{max} = 0.64 \cdot 10^{-1} \cdot 2 = 1.28\ dW$  

Nel caso ideale l'induttore prende in presito energia nella prima meta' del periodo, per poi restiurla al circuito nella seconda meta', si parla quindi di potenza reattiva in quanto non viene trasformata ma solo scambiata.  

![sine_current_solenoid_5](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/23ea4664-e384-4f74-8192-7f50bf0692a5)  
