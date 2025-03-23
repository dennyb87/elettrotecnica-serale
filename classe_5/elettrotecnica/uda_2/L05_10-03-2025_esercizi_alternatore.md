# Esercizio alternatore  

Dati di targa:  

```math
2P = 6\\
f_n = 50\ Hz\\
S_n = 20\ kVA\\
V_n = 400\ V\\
```
Dalla **prima prova** a vuoto si ha che:  

$I_e = 6.5\ A$
$V_{0f} = 260\ V$

Dalla seconda si ha:  

$I_e =2\ A$  
$I_{cc} = 40\ A$  

Le fasi statoriche sono collegate a stella e $R_i = 0.243\ \Omega$ ed infine le potenze perse conosciute sono:  

$P_{av} = 240\ W$  
$P_{fn} = 340\ W$  
$P_{add} \simeq 0\ W$  

Sapendo che l'alternatore funziona con $I_e = 6.5\ A$ e $V_e = 80\ V$ ed eroga $I = \frac{4}{5}I_n$ ad un carico **RL** con fattore di potenza $\cos\varphi = 0.75$ si vuole trovare:

* corrente di cortocircuito $I_{cc}$
* tensione concatenata $V$
* potenza assorbita $P_a$
* rendimento $\eta$
* coppia motrice $C_m$
* coppia resistente $C_r$

## Soluzione  

La corrente di eccitazione $I_e = 6.5\ A$ della prova a vuoto coincide con quella di funzionamento per cui sappiamo anche che $E_0 = V_{0f} = 260\ V$  

### Corrente di cortocircuito  

Conoscendo la corrente di cortocircuito di una delle prove, grazie all'ipotesi di linearita' possiamo utilizzare le proporzioni per ricavare $I_{cc}$ di funzionamento:  

$\dfrac{I_{e1}}{I_{cc1}} = \dfrac{6.5}{I_{cc}} \implies I_{cc} = \dfrac{I_{cc1}}{I_{e1}}\cdot 6.5 = \dfrac{40}{2}\cdot 6.5 \simeq 130\ A$  

### Tensione concatenata  

Troviamo la corrente erogata grazie alla frazione di carico $\alpha = \frac{4}{5}$  

$I_n = \dfrac{S_n}{\sqrt{3}\cdot V_n} = \dfrac{20\cdot10^3}{\sqrt{3}\cdot 400} \simeq 28.87\ A$  

$I = \frac{4}{5}I_n = \frac{4}{5}\cdot 28.87 \simeq 23.1\ A$  

Ricaviamo $X_s$ da $Z_s$ sapendo che...  

$Z_s = \dfrac{E_0}{I_{cc}} = \dfrac{260}{130} = 2\ \Omega$  

$X_s = \sqrt{Z_s^2-R_i^2} = \sqrt{2^2-0.243^2} \simeq 1.99\ \Omega$  

Ricaviamo infine $V_f$ dalla formula:  

$E_0^2 = \bigg(V_f\cdot\cos\varphi+R_iI\bigg)^2+\bigg(V_f\cdot\sin\varphi+X_sI\bigg)^2$  

$260^2 = \bigg(V_f\cdot 0.75+0.243\cdot 23.1\bigg)^2+\bigg(V_f\cdot 0.66+1.99\cdot 23.1 \bigg)^2$  

Espandendo i quadrati di binomi e applicando la quadratica otteniamo la tensione di fase statorica:  

$V_f \simeq 223.8\ V$  

Essendo le fasi statoriche collegate a stella si ha infine che la tensione concatenata e':  

$V = \sqrt{3}\cdot V_f = \sqrt{3}\cdot 223.8 \simeq 387.63\ V$  

### Potenza assorbita  

Sappiamo che la potenza utile e':  

$P = \sqrt{3}VI\cos\varphi = \sqrt{3}\cdot 387.63 \cdot 23.1 \cdot 0.75 \simeq 11631.92\ W$  

$P_{j1} = 3R_iI^2 = 3\cdot 0.243 \cdot 23.1^2 = 389\ W$  

$P_f = P_{fn}\bigg(\dfrac{V}{V_n}\bigg)^2 = 340\cdot\dfrac{387.63^2}{400^2}\simeq 319.3\ W$  

$P_e = V_e \cdot I_e = 80\cdot 6.5 = 520$

Allora la potenza assorbita sara'...  

$P_a = P + P_{j1} + P_f + P_{av} + P_e = 11631.92 + 389 + 319.3 + 240 + 520 = 13100.22\ W$  

### Rendimento  

$\eta = \dfrac{P}{P_a} = \dfrac{11631.92}{13100.22} \simeq 0.89$  

### Coppia motrice e resistente  

$n = \dfrac{60f}{P} = \dfrac{60\cdot 50}{3} = 1000\ \text{rpm}$  

$C_m = \dfrac{60P_a}{2\pi n} = \dfrac{60\cdot 13100.22}{2\pi \cdot 1000} \simeq 125.1\ Nm$  

$C_r = \dfrac{60P}{2\pi n} = \dfrac{60\cdot 11631.92}{2\pi \cdot 1000} \simeq 111.07\ Nm$  
