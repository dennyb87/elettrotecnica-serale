# Tensioni nel generatore elettrico trifase  

![three_phase_schema](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/d01e3fd8-5a06-4c89-92d1-2e9a437be5f6)  

Sapendo che le tre tensioni non sono in fase tra loro, si vuole esaminare il grafico delle tensioni nel tempo notando che la differenza di tensione tra due poli e' rappresentata dal modulo della differenza vettoriale delle tensioni.  

![votlage_diff](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c080162d-e586-476b-a4cc-ba913905fea2)  

$\vec{V}_{12} = \vec{E_1} - \vec{E_2}$  

$\vec{V}_{23} = \vec{E_2} - \vec{E_3}$  

$\vec{V}_{31} = \vec{E_3} - \vec{E_1}$  

Ma $\vec{E}_1 - \vec{E}_2 = \vec{E}_1 + (-\vec{E}_2)$ percio' e' sufficiente fare la somma vettoriale dei vettori opposti, ottenendo quindi un altro **sistema simmetrico di tensioni** sfasate di $30^\circ$ rispetto al primo.  

![line_voltage_derivation](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/3389fbc5-3835-4749-9b11-5bb2caf5e399)  

Per la regola del parallelogramma sappiamo che $V_{12}$ e' la base di un triangolo isoscele che ha per lato $E_1$ e allora...  

$V_{12} = 2 \cdot E_1\cos \alpha = 2 \cdot E_1 \cos 30^\circ = \cancel{2} \cdot E_1 \dfrac{\sqrt{3}}{\cancel{2}} = E_1\sqrt{3}$  

Generalizzando si ha che...  

$E = E_1 = E_2 = E_3$  
$V = V_{12} = V_{23} = V_{31}$  

Dove $E$ prende il nome di **tensione di fase** mentre $V = E\sqrt{3}$ e prende il nome di **tensione di linea**.  
