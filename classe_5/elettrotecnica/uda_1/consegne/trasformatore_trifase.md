# Trasformatore trifase  

Un trasformatore ha i seguenti dati di targa:  

```math
\begin{aligned}
    S_n &= 25\ kVA \\
    K_0 &= \dfrac{6\ kV}{0.4\ kV} = 15\ \text{(collegamento Dy)}  \\
    P_{0\%} &= 1.5\ \% \\
    \cos\varphi_0 &= 0.25 \\
    P_{cc\%} &= 2\ \% \\
    \cos\varphi_{cc} &= 0.42
\end{aligned}
```

Il trasformatore alimenta due carichi in parallelo con una tensione $V_2 = 380\ V$. Il primo a stella di tipo **RL** che assorbe $P_{21} = 12\ kW$ con $\cos\varphi_{21} =0.8$, mentre il secondo a triangolo che assorbe $P_{22} = 9\ kW$.  

Calcolare:  
1. i parametri longitudinali e trasversali al primario e scondario
2. la corrente $I_2$ assorbita sul lato BT
3. la tensione concatenata $V_1$ di alimentazione
4. le perdite nel ferro e nel rame e il rendimento nelle condizioni di funzionamento
5. la corrente $I_1$ assorbita sul lato MT ed il fattore di potenza primario $\cos\varphi_1$  

## 1 - Parametri longitudinali  

```math
P_{cc} = \dfrac{P_{cc\%}\cdot S_n}{100} = \dfrac{2\cdot 25\ 000}{100} = 500\ W  
```

$I_{1n} = \dfrac{S_n}{\sqrt{3}\cdot V_{1n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 6\ 000} \simeq 2.41\ A$  

$I_{2n} = \dfrac{S_n}{\sqrt{3}\cdot V_{20n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 400} \simeq 36.08\ A$  

$R_{1cc} = \dfrac{P_{cc}}{3\cdot I_{1n}^2} = \dfrac{500}{3\cdot 2.41^2} \simeq 28.7\ \Omega$  

$R_{2cc} = \dfrac{P_{cc}}{3\cdot I_{2n}^2} = \dfrac{500}{3\cdot 36.08^2} \simeq 0.128\ \Omega$  

$X_{1cc} = R_{1cc}\cdot \tan\varphi_{cc} = 28.7\cdot 2.16 \simeq 62\ \Omega$  

$X_{2cc} = R_{2cc}\cdot \tan\varphi_{cc} = 0.128\cdot 2.16 \simeq 0.276\ \Omega$  

## 1 - Parametri trasversali  

```math
P_0 = \dfrac{P_{0\%}\cdot S_n}{100} = \dfrac{1.5\cdot 25\ 000}{100} = 375\ W
```

$Q_0 = P_0\cdot\tan\varphi_0 = 375\cdot 3.87 = 1451.25\ VAR$  

$G_0 = \dfrac{P_0}{V_{1n}^2} = \dfrac{375}{6\ 000^2} = 10.42\ \mu S$  

$B_0 = \dfrac{Q_0}{V_{1n}^2} = \dfrac{1451.25}{6\ 000^2} \simeq 40.3\ \mu S$  

$G_0^{''} = G_0\cdot K_0^2 = 10.42\cdot 15^2 \simeq 2.34\ mS$  

$B_0^{''} = B_0\cdot K_0^2 = 40.3\cdot 15^2 = 9.07\ mS$  

## 2 - Corrente assorbita lato BT  

Trattandosi di carichi non puramente resistivi utilizziamo *Boucherot* per trovare la corrente $I_2$  

$P_2 = P_{21} + P_{22} = 12 + 9 = 21\ kW$  

$Q_2 = Q_{21} = P_{21}\cdot\tan\varphi_{21} = 12\cdot 0.75 = 9\ kVAR$  

$I_2 = \dfrac{S_2}{\sqrt{3}\cdot V_2} = \dfrac{\sqrt{P_2^2+Q_2^2}}{\sqrt{3}\cdot V_2} = \dfrac{\sqrt{21^2+9^2}}{\sqrt{3}\cdot 380} \simeq 34.71\ A$  

## 3 - Tensione concatenata $V_1$ di alimentazione  

Per trovare $V_1$ occorre prima trovare $V_{20} = \Delta V + V_2$ e quindi $\cos\varphi_2$ per cui...  

$\cos\varphi_2 = \dfrac{P_2}{S_2} = \dfrac{21\ 000}{22\ 847.32} \simeq 0.92$  

$\sin\varphi_2 \simeq 0.39$  

$\Delta V = \sqrt{3}\cdot I_2(R_{2cc}\cos\varphi_2+X_{2cc}\sin\varphi_2) = \sqrt{3}\cdot 34.71(0.128\cdot0.92+0.276\cdot0.39) \simeq 13.55\ V$  

$V_{20} = \Delta V + V_2 = 13.55 + 380 = 393.55\ V$  

$V_1 = V_{20}\cdot K_0 = 393.55\cdot 15 = 5903.25\ V$  

## 4 - Perdite nel ferro, nel rame e rendimento  

$P_f = P_0\bigg(\dfrac{V_1}{V_{1n}}\bigg)^2 = 375 \cdot\bigg(\dfrac{5\ 903.25}{6\ 000}\bigg)^2 \simeq 363\ W$  

$P_{cu} = P_{cc}\bigg(\dfrac{I_2}{I_{2n}}\bigg)^2 = 500\cdot\bigg(\dfrac{34.71}{36.08}\bigg)^2 \simeq 462.75\ W$  

$\eta = \dfrac{P_2}{P_1} = \dfrac{P_2}{P_2+P_f+P_{cu}} = \dfrac{21\ 000}{21\ 000 + 363 + 462.75} = \dfrac{21\ 000}{21\ 825.75} = \simeq 0.962 \implies 96.2\ \%$  

## 5 - Corrente assorbita lato MT e fattore di potenza  

$Q_\mu = P_f\cdot\tan\varphi_0 = 363\cdot 3.87 \simeq 1.4\ kVAR$  

$Q_1 = Q_2+Q_\mu+3X_{2cc}\cdot I_2^2 = 9\ 000+1400+3\cdot 0.276 \cdot 34.71 \simeq 11.4\ kVAR$  

$S_1 = \sqrt{P_1^2+Q_1^2} = \sqrt{21.83^2+11.4^2} \simeq 24.63\ kVA$  

$I_1 = \dfrac{S_1}{\sqrt{3}\cdot V_1} \dfrac{24.63}{\sqrt{3}\cdot 5.9} \simeq 2.41\ A$  

$\cos\varphi_1 = \dfrac{P_1}{S_1} = \dfrac{21.83}{24.63} \simeq 0.886$  
