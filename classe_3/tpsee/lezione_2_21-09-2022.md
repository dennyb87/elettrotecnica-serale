# Corrente alternata 

Tracciando su un grafico il comportamento della corrente (o della tensione) nel tempo si ottiene una sinusoide.
Il tempo necessario al completamento di un ciclo (per esempio da picco a picco) si chiama **periodo**, si rappresenta con $T$, e si misura in secondi e.g. $T = 0.8s$.  
Se per completare $1$ ciclo si impiegano $0.8$ secondi, significa che in un secondo si completano $1.25$ cicli.  
Questa e' in effetti la definizione di frequenza, ovvero cicli al secondo $f = \frac{cicli}{secondi} = \frac{1}{T} = \frac{1}{0.8} = 1.25 Hz$.  
La corrente alternata viene fornita ad una frequenza di $50$ cicli al secondo $f = \frac{50}{1} = 50Hz$.  

Va da se che per trovare il periodo e' sufficiente $T = \frac{1}{frequenza} = \frac{1}{1.25Hz} = 1 \cdot \frac{0.8}{1} = 0.8s$.  
Significa che il periodo (o tempo di completamento di un ciclo) della corrente alterna e' di $T = \frac{1}{50Hz} = 0.02s = 20ms$.

![periodo](https://user-images.githubusercontent.com/7195133/195782788-20176d0f-41f1-4095-9c3f-170160c01631.png)  



## Valore efficace  

Una corrente alternata per sua natura varia nel tempo, per evitare di dover analizzare il suo valore istante per istante, si utlizza il cosiddetto **valore efficace**, che e' quel valore che avrebbe una corrente continua che produce lo stesso effetto termico.  

![valore_efficace](https://user-images.githubusercontent.com/7195133/195953368-c68f168e-acb4-479c-9a65-138f53186909.png)  

Il valore efficace $V_{eff}$ si ottiene dividendo il valore di picco per la radice quadrata di 2.  

$V_{eff} = \frac{V_p}{\sqrt{2}}$  
$V_p = V_{eff} \cdot \sqrt{2}$

Approssimativamente quindi $V_{eff} \simeq V_p \cdot 0.707$ mentre $V_p \simeq V_{eff} \cdot 1.414$


## Classificazione dei sistemi elettrici  

 |categoria|AC|CC|tipo di tensione|sigla|
 |--|--|--|--|--|
 |0 (zero)|$x \leq 50V\sim$|$x \leq 120V\overline{...}$|bassissima|BBT|
 |1 (prima)|$50V \lt x \leq 1000V\sim$|$120V \lt x \leq 1500V\overline{...}$|bassa|BT|
 |2 (seconda)|$1000V \lt x \leq 30kV\sim$|$1500V \lt x \leq 30kV$|media|MT
 |3 (terza)|$30kV \lt x \leq 130kV$||alta|AT|
 |3 (quarta)|$x \gt 130kV$||altissima|AAT|

