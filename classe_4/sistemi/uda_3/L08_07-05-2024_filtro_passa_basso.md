# Partitore di tensione  

In un circuito puramento ohmico non si ha nessuna risposta in frequenza, ovvero il sitema non risponde in alcun modo alle variazioni di frequenza.  

![voltage_divider](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/680466fb-9638-4831-b5f9-564258df18e8)  

$R_a = 3\ \Omega$  
$R_b = 1\ \Omega$  

$G(s) = \dfrac{V_{out}}{V_{in}} =  \cdot \dfrac{\cancel{V_{in}}R_b}{R_a+R_b} \cdot \dfrac{1}{\cancel{V_{in}}} = \dfrac{R_b}{R_a+R_b} = \dfrac{1}{3+1} = \dfrac{1}{4}$  

Nessun termine dipende dalla frequenza, di conseguenza il sistema e' un riduttore di tensione, ovvero si ha in uscita una tensione minore di quella in ingresso che dipende unicamente dalla configurazione dei resistori.  
Di seguito i grafici in continua $\omega = 0$ e alternata $\omega > 0$ in cui la tensione in uscita e' sempre $\dfrac{V_{in}}{4}$  

![sistema_ohmico_continua](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a2ae1310-5563-43b8-8c99-c91731431fc6)  

![sistema_ohmico_alternata](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/83601a68-f579-4ca2-92fb-50953d69e115)  

# Filtro passa-basso  

![filtro_passa_basso](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ec2b9437-f7ed-471f-87d3-45cc3de6a198)  

In un circuito di questo tipo si ha che l'impedenza dell'induttore varia al variare della frequenza, per cui si ha in effetti una risposta in frequenza, ovvero la funzione di trasferimento varia al variare dalla frequenza.  

$L = 5\ H$  
$R = 2\ \Omega$  

$G(s) = \dfrac{\cancel{V_i}R}{R+Ls} \cdot \dfrac{1}{\cancel{V_i}} = \dfrac{R}{R+Ls} = \dfrac{2}{2 + 5s} = 0.4 \cdot \dfrac{1}{s + 0.4}$  

Per trovare $G$ e' necessario valutare $G(s)|_{s = j\omega}$ ovvero...  

$G(j\omega) = \dfrac{R}{R+j\omega L}$  

Ma $R+j\omega L$ e' un numero complesso, allora per *De Moivre* si cha che il quoziente tra due numeri complessi e' il quoziente tra i loro moduli e la differenza tra i rispettivi angoli. Il numeratore non ha parte complessa quindi il modulo coincide con $R$ mentre al denominatore si applica il teorema di Pitagora...  

$|G| = \dfrac{R}{\sqrt{R^2+X^2_L}} = \dfrac{R}{\sqrt{R^2+(\omega L)^2)}} = \dfrac{R}{\sqrt{R^2+(2\pi f L)^2}}$  

Allora tracciando $|G|$ al variare della frequenza $f$ otteniamo una curva di questo tipo...  

$|G| = \dfrac{2}{\sqrt{2^2+(2\pi f5)}}$  

![freq_response](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/bf20208a-dcbb-446e-a8d9-079192ec9dc7)  

![low_pass_filter_characteristics](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b81e8c2c-a133-475a-a39d-7be97c349afd)  

La risposta in frequenza sara' allora di questo tipo, dove per $\omega = 0$ ovvero in continua, l'induttore non presenta impedenza, per cui $V_{o} = V_{i} \implies G = 1$  

Quando $\omega = a_G = 0.4\ \frac{rad}{s}$ si ha la frequenza di taglio, *cut-off frequency* $f_c$ in questo caso $f_c = \dfrac{a_G}{2\pi} = \dfrac{0.4}{2\pi} \simeq 0.064\ Hz$ dove $G = \dfrac{1}{\sqrt{2}}$ e comincia a descrescere in modo significativo.  

Questo tipo di circuito prende il nome di **filtro passa-basso** in quanto lascia passare il segnale a frequenze basse, mentre quelle alte vengono soppresse.  

| $f[Hz]$ | $V_{in}[V]$ | $V_{out}[V]$ | $G$  |
| ------- | ----------- | ------------ | ---- |
| 0       | 10          | 10           | 1    |
| 0.1     | 10          | 5            | 0.5  |
| 0.5     | 10          | 1.2          | 0.12 |
| 1       | 10          | 0.6          | 0.06 |

Di seguito i grafici delle righe in tabella.  

![low_pass_filter_0Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/966e51c9-91e0-4f9a-aaaa-a501fdd45166)  

![low_pass_filter_0 1Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/d9c8675b-3bff-4844-ac98-773f45c391b2)  

![low_pass_filter_0 5Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/598b19dd-402e-4cab-97b7-a729dfd673bc)  

![low_pass_filter_1Hz](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f25ab466-c92e-44fc-84fb-844ce3db6330)  

