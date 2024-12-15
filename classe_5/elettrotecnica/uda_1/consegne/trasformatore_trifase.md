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

$P_{cc} = \dfrac{P_{cc\%}\cdot S_n}{100} = \dfrac{2\cdot 25\ 000}{100} = 500\ W$  

$I_{1n} = \dfrac{S_n}{\sqrt{3}\cdot V_{1n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 6\ 000} \simeq 2.41\ A$  

$I_{2n} = \dfrac{S_n}{\sqrt{3}\cdot V_{20n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 400} \simeq 36.08\ A$  

$R_{1cc} = \dfrac{P_{cc}}{3\cdot I_{1n}^2} = \dfrac{500}{3\cdot 2.41^2} \simeq 28.7\ \Omega$  

$R_{2cc} = \dfrac{P_{cc}}{3\cdot I_{2n}^2} = \dfrac{500}{3\cdot 36.08^2} \simeq 0.128\ \Omega$  

$X_{1cc} = R_{1cc}\cdot \tan\varphi_{cc} = 28.7\cdot 2.16 \simeq 62\ \Omega$  

$X_{2cc} = R_{2cc}\cdot \tan\varphi_{cc} = 0.128\cdot 2.16 \simeq 0.276\ \Omega$  

## 1 - Parametri trasversali  

$P_0 = \dfrac{P_{0\%}\cdot S_n}{100} = \dfrac{1.5\cdot 25\ 000}{100} = 375\ W$  

$Q_0 = P_0\cdot\tan\varphi_0 = 375\cdot 3.87 = 1451.25\ VAR$  

$G_0 = \dfrac{P_0}{V_{1n}^2} = \dfrac{375}{6\ 000^2} = 10.42\ \mu S$  

$B_0 = \dfrac{Q_0}{V_{1n}^2} = \dfrac{1451.25}{6\ 000^2} \simeq 40.3\ \mu S$  

$G_0^{''} = G_0\cdot K_0^2 = 10.42\cdot 15^2 \simeq 2.34\ mS$  

$B_0^{''} = B_0\cdot K_0^2 = 40.3\cdot 15^2 = 9.07\ mS$  

## 2 - Corrente assorbita lato BT  

Trattandosi di carichi non puramente resistivi utilizziamo *Boucherot* per trovare la corrente $I_2$  

$P_2 = P_{21} + P_{22} = 12 + 9 = 21\ kW$  

$Q_{21} = P_{21}\cdot\tan\varphi_{21} = 12\cdot 0.75 = 9\ kVAR$  

$I_2 = \dfrac{\sqrt{P_2^2+Q_{21}^2}}{\sqrt{3}\cdot V_2} = \dfrac{\sqrt{21^2+9^2}}{\sqrt{3}\cdot 380} \simeq 34.71\ A$  
