# Parametri di cortocircuito  

![real_transformer_no_load](https://github.com/user-attachments/assets/ad19ca32-d0c6-4d31-b2e2-8dd95eb788d8)  

Si ha un trasformatore con:  

* $K_0 = \dfrac{V_{in}}{V_{20n}} = \dfrac{5000}{250} = 20\ V$
* $I_0 = 2\ A$
* $\cos \varphi = 0.2$
* $R_1 = 1.8\ \Omega$
* $X_1 = 3.6\ \Omega$
* $R_2 = 5\ m\Omega$
* $X_2 = 9\ m\Omega$

![parametri_cortocircuito](https://github.com/user-attachments/assets/68067eb1-0484-468e-8e7b-37fc4bb8a83c)    

Per semplificare il circuito e' possibile spostare i parametri longitudinali dal primario al secondario e viceversa. In questo caso il parametro $R_{1cc}$ e' composto da:  

$R_{1cc} = R_1 + R_{2^\prime}$  

Dove $R_1$ e' la resistenza originariamente presente sul primario, mentre $R_{2^\prime}$ e' la resistenza del secondario spostata sul primario. Per ottenere la resistenza equivalente e' necessario moltiplicare o dividere la resistenza originale per $K_0^2 \simeq K_N^2$ in dipendenza della variazione del numero di spire.  

In questo caso spostando $R_2$ dal secondario al primario, il numero di spire e' aumentato in quanto $V_{in} > V_{20n}$ per cui si moltiplica per $K_0$  

$R_{2^\prime} = R_2 \cdot K_0^2 = 5 \cdot 10^{-3} \cdot 20^2 = 2\ \Omega$  

$X_{2^\prime} = X_2 \cdot K_0^2 = 9 \cdot 10^{-3} \cdot 20 = 0.18\ \Omega$  

$R_{1cc} = R_1 + R_{2^\prime} = 1.8 + 2 = 3.8\ \Omega$  

$X_{1cc} = X_1 + X_{2^\prime} = 3.6 + 0.18 = 3.78\ \Omega$  

Per ottenere i parametri equivalenti sul secondario si utilizza lo stesso sistema con la differenza che i parametri in questo caso vanno moltiplicati per $\dfrac{1}{K_0}$  

$R_{2cc} = R_2 + R_{1^{\prime\prime}} = R_2 + R_1 \cdot \dfrac{1}{K_0}$  

$X_{1cc} = X_2 + X_{1^{\prime\prime}} = X_2 + X_1 \cdot \dfrac{1}{K_0}$  

### Perdite nel ferro  

Conoscendo $I_0$ e' possibile calcolare le perdite nel ferro alla tensione nominale con:  

$P_0 = V_{in}\cdot I_0\cdot\cos\varphi = 5000 \cdot 2 \cdot 0.2 = 2000\ W$  

Conoscendo la formula generale per il calcolo delle perdite nel ferro...  

$P_{fe} = G_0 \cdot E_1^2$  

Dove $G_0 = \dfrac{1}{R_0}$ ovvero l'ammettenza (unita' di misura *siemens* $[S]$) del parametro reistivo trasversale, si ha infine che...  

$G_0 = \dfrac{P_0}{E_1^2} = \dfrac{2000}{5000^2} = 80\ \mu S$  

Trovato $G_0$ grazie alla formula generale e' possibile stimare quali siano le perdite a diverse tensioni in ingresso...  

$P_{fe} = G_0 \cdot E_1^2 = 80 \cdot 10^{-6} \cdot 4000^2 = 1280\ W$  

### Potenza reattiva nel ferro  

$Q_{fe} = B_0 \cdot E_1^2$  

Dove $B_0 = \dfrac{1}{X_0}$ ovvero la suscettanza (sempre in *siemens* $S$) del parametro reattivo trasversale. Per il triangolo delle potenze si ha allora che...  

![powers_triangle](https://github.com/user-attachments/assets/af77f5c5-3534-456d-ae41-8e4554902c91)  

$\varphi = \arccos(\cos \varphi) = \arccos(0.2) \simeq 78.463^\circ$  
$\tan \varphi = \tan (78.463) \simeq 4.9$
$Q_0 = P_0 \cdot \tan\varphi = 2000 \cdot 4.9 = 9800\ VAR$  
