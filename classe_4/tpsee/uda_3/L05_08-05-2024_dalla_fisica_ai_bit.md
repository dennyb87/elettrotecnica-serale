# Dalla grandezza fisica ai bit  

Si vuole esaminare il processo di conversione analogico-digitale partendo da una grandezza fisica come la temperatura. Scegliamo una sonda **PT1000** che sappiamo essere riconducibile ad un resistore di resistenza variable, in questo caso in dipendenza della temperatura.  

## Trasduttore  

![pt1000](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/65bb1416-008e-4485-b79f-7cc7065085d1)  

La sonda dovra' essere inserita in un circuito di condizionamento che servira' per fornire un'interfaccia standard, in particolare $0 \div 10\ V$ in uscita (alternativamente $0 \div 20\ mA$ in corrente).  

![circuito_condizionamento](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b764bad1-7220-49fe-a04b-41343648b458)  

In figura si puo' dedurre che la temperatura sia $0^\circ$ in quanto la sonda $R_T = 1\ k\Omega$  
Per il partitore di tensione in questa configurazione si hanno $V_{out} = 5\ V$ in uscita, mentre nei casi limite si ha rispettivamente:  

| $R_T[\Omega]$ | $V_{out}[V]$ |
| ------------- | ------------ |
| $0$           | $0$          |
| $\infty$      | $10$         |

```mermaid
flowchart LR
    energy--->pt1000
    subgraph trasduttore
        pt1000---cond["circuito di condizionamento"]
    end
    trasduttore--"0 ÷ 10V"--->out(" ")
```

Abbiamo quindi un dispositivo in grado di fornire un segnale analogico standard, in particolare infiniti valori $0 \div 10\ V$ al variare della temperatura. Adesso non ci resta che convertire il segnale analogico in un segnale digitale.  

## Convertitore analogico-digitale  

Nella conversione verra' necessariamente persa dell'informazione in quanto gli infiniti valori $0 \div 10\ V$ verranno mappati in un numero finito di valori. In questo caso per semplicita' si vogliono usare 3 bit, per un totale di $2^3$ quanti.  

$Q = \dfrac{V_{Fs}}{N} = \dfrac{10}{2^3} = 1.25\ V$  

Si noti come la scala sia sfasata di mezzo quanto $0.625$  

![adc_function](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c49e3d63-92ac-4b30-b72c-071b504a62ea)  

Questo a livello pratico e' riproducibile con una serie di comparatori e resistenze opportunamente collegati, che servendosi di una rete logica, l'*encoder* in figura, convertono il segnale analogico $0 \div 10\ V$ in un segnale digitale binario a 3 bit.  

![3_bit_adc](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/89b3faeb-0920-4d2f-a707-3011e2d3cfcd)  
