# Legge di Ohm generalizzata  

Dopo aver esaminato il comportamento di un circuito puramente capacitivo vogliamo formalizzare la legge di Ohm generalizzata:  

$\vec{Z} = \dfrac{\vec{V}}{\vec{I}} = \dfrac{V\angle\theta_V}{I\angle\theta_I} = Z\angle\theta$  

Dove $Z = \dfrac{V}{I}$ ovvero il rapporto tra i moduli di tensione e corrente, mentre $\theta = |\theta_V - \theta_I|$ ovvero l'angolo di sfasamente tra tensione e corrente. In generale si ha che l'impedenza e' uguale a:  

$\vec{Z} = R + jX$  

![impedance_triangle](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/63adc465-b403-47c9-8046-ffb5048233eb)  

![reactance_vs_resistance_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/27307838-c2b1-4bc7-bed0-189c44b2b9c8)  

$X_c = \dfrac{1}{\omega \cdot C}$  

Al contrario della resistenza, che resta costante al variare della frequenza, la reattanza capacitiva segue un andamento inversamente proporzionale per cui:  

$f \to 0 \implies \omega \to 0 \implies X_c \to \infty$  

$f \to \infty \implies \omega \to \infty \implies X_c \to 0$  

Ne segue che in continua dove $f = 0\ Hz$ si presenta una reattanza capacitiva tale da impedire totalemente qualunque spostamento di cariche.  

## Circuito ohmico-capacitivo  

![ohmico_capacitivo_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/26da28e8-bf99-4fa8-9a74-633ce463d607)  

Conoscendo la reattanza del condensatore a questo regime $X_c \simeq 3.185\ \Omega$ possiamo risolvere questo tipo di circuito cominciando con il calcolo dell'impedenza:  

$\theta = \tan^{-1}\frac{X_c}{R} = \tan^{-1}\frac{3.185}{4} \simeq 38.529^\circ$  

$Z = \dfrac{R}{\cos\theta} = \dfrac{4}{0.782} = 5.115\ \Omega$  

Troviamo infine la corrente...  

$I = \dfrac{V}{Z} = \dfrac{10}{5.155} = 1.955\ A$  

