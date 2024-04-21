# Scomposizioni per antitrasformate  

Dato un circuito RL serie con:  

$R_1 = 1\ \Omega$  
$R_2 = 3\ \Omega$  
$L = 2\ H$  
$E(s) = \dfrac{10}{s}$  

Per il partitore di tensione si ha in uscita:  

$V_u(s) = V_i(s) \cdot \dfrac{R_2 + Ls}{R_1+R_2+Ls}$  

$V_u(s) = \dfrac{10}{s} \cdot \dfrac{3+2s}{4+2s} = \dfrac{10}{s} \cdot \dfrac{\cancel{2}(s+\frac{3}{2})}{\cancel{2}(s+2)} = \dfrac{10s+15}{s^2+2s}$  

Sappiamo pero' che la frazione puo' essere scomposta...  

$V_u(s) = \dfrac{A}{s} + \dfrac{B}{s+2}$  

Per trovare $A$ sara' allora sufficiente moltiplicare entrambe i membri per il denominatore dell'icognita da individuare e infine porre $s$ tale che annulli il denominatore, in questo caso $s = 0$  

$s \cdot V_u(s) = \dfrac{A}{\cancel{s}} \cdot \cancel{s} + \dfrac{B}{s+2} \cdot \cancel{}s$  

$A = \bigg[s \cdot V_u(s)\bigg]_{s = 0} = A + \dfrac{B}{0 + 2} \cdot 0$  

Sostituendo i valori...  

$A = \bigg[s \cdot V_u(s)\bigg]_{s = 0} = \cancel{s} \cdot \dfrac{10}{\cancel{s}} \cdot \dfrac{3+2s}{2(s+2)} = 10 \cdot \dfrac{3+0}{4+0} = 7.5$  

$B = \bigg[(s+2) \cdot V_u(s)\bigg]_{s = -2} = \cancel{s+2} \cdot \dfrac{10}{s} \cdot \dfrac{3+2s}{2\cancel{(s+2)}} = \dfrac{10(3+2(-2))}{2(-2)} = 2.5$  

Troviamo allora che...  

$V_u(s) = \dfrac{7.5}{s} + \dfrac{2.5}{s+2} \implies v_u(t) = 7.5u(t) + 2.5 \cdot e^{-2t}u(t)$  

![response_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/42b2b477-4e8e-42d0-829f-923d7f10a419)  

In generale le costanti di tempo sono date dai poli, in questo caso:  

$a = \dfrac{R_1+R_2}{L} \implies \tau = \dfrac{1}{a} = \dfrac{L}{R_1+R_2} = \dfrac{2}{4} = 0.5\ s$  

$T_d = 5\tau = 5 \cdot 0.5 = 2.5\ s$  

Infine l'analisi della funzione di trasferimento ci conferma che il sistema e' **stabile** in quanto gli zeri e i poli sono negativi.  

$G(s) = \cancel{V_i(s)} \cdot \dfrac{R_2 + Ls}{R_1+R_2+Ls} \cdot \dfrac{1}{\cancel{V_i(s)}} = \dfrac{s + \frac{3}{2}}{s+2}$  

$s_0 = -\frac{3}{2}$  
$s_{p_1} = -2$  

![zeroes_and_poles](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/98961b1c-d642-49a2-83c3-b5dc858b8492)  
