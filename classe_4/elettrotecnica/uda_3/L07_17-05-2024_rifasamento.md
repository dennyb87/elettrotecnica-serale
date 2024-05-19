# Rifasamento  

Rifasare un impianto significa riportare in fase tensione $\vec{V}$ e corrente $\vec{I}$. I questo caso si vuole effettuare il rifasamento di un carico ohmico-induttivo.  

![phase_shift_pre_fix](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/981331b9-16b9-4f44-a494-dd31346e927a)  

$E_{max} = 142\ V \implies V = \dfrac{E}{\sqrt{2}} = \dfrac{142}{\sqrt{2}} \simeq 100\ V$  

$X_L = \omega L = 2 \pi fL= 2 \pi \cdot 0.64 \cdot 1 \simeq 4\ \Omega$  

Per il teorema di Pitagora si ha allora che $Z = 5\ \Omega$  

$I = \dfrac{V}{Z} = \dfrac{100}{5} = 20\ A$  

$\varphi = \tan^{-1}(\frac{4}{3}) \simeq 53.13^\circ$  

Considerando che la corrente e' in ritardo di $53.13^\circ$ si vuole trovare il vettore $\vec{I_C}$ tale che la somma vettoriale con $\vec{I_L}$ dia come risultato il vettore $\vec{I}$ in fase con $\vec{V}$. Per la trigonometria si ha allora che...  

![phase_shift_vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c11c659b-f9bb-4ab0-a025-6bbf84b35b35)  

$I_C = I_L \cdot \sin \varphi = 20 \cdot \sin 53.13^\circ \simeq 16\ A$  

Trovata la corrente necessaria per rifasare il circuito non resta che risolvere per $X_C$ trovando la capacita' del condensatore di bypass da inserire nel circuito.  

$X_C = \dfrac{V}{I_C} = \dfrac{100}{16} = 6.25\ \Omega$  

![phase_shift_post_fix](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/4813a40b-0344-44cb-8b28-47b534f15035)  

Inserito nel circuito scopriamo, per il teorema di *Boucherot*, che le potenze reattive si bilanciano, e la potenza attiva resta invariata, ottenendo una corrente rifasata $I_{RIF}$ ridotta.  

$P_R = RI^2_L = 3 \cdot 20^2 = 1200\ W$  
$Q_L = X_LI^2_L = 4 \cdot 20^2 = 1600\ VAR$  
$Q_C = X_CI^2_C = 6.25 \cdot 16^2 = 1600\ VAR$  

$P_{tot} = P_R = 1200\ W$  
$Q_{tot} = Q_L - Q_C = 1600 - 1600 = 0\ VAR$  

$I_{RIF} = \dfrac{P}{V} = \dfrac{1200}{100} = 12\ A$  
