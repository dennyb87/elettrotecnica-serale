# Esercizio trasformatore trifase  

Si ha un trasformatore con i seguenti dati di targa:  

```math
\begin{aligned}
S_n &= 25\ kVA\\
V_{1n} &= 10\ kV\\
V_{20n} &= 400\ V\\
K_0 &= 25\\
P_{0\%} &= 1.5\ \%\\
\cos\varphi_0 &= 0.25\\
P_{cc\%} &= 2.5\ \%\\
\cos\varphi_{cc} &= 0.42
\end{aligned}
```

Il trasformatore e' alimentato sul lato AT alla tensione nominale ma con frazione di carico $\alpha = \frac{4}{5}$ ed un $\cos\varphi_2 = 0.8$ **RL**.  

Calcolare:  

1. paramentri longitudinali e trasversali
2. la caduta di tensione percentuale e la tensione sul carico
3. la potenza attiva consumata dal carico e il rendimento
4. l'impedenza di ogni fase del carico supposto equilibrato e collegato a triangolo

## 1 - Parametri longitudinali  

```math
P_{cc} = \dfrac{P_{cc\%}\cdot S_n}{100} = \dfrac{2.5\cdot 25\ 000}{100} = 625\ W
```

Dato che nel trifase $S_n = \sqrt{3}\cdot V_{1n}\cdot I_{1n} = \sqrt{3}\cdot V_{20n}\cdot I_{2n}$ allora...  

$I_{1n} = \dfrac{S_n}{\sqrt{3}V_{1n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 10\ 000} \simeq 1.44\ A$  

$I_{2n} = \dfrac{S_n}{\sqrt{3}V_{20n}} = \dfrac{25\ 000}{\sqrt{3}\cdot 400} \simeq 36.08\ A$  

Dato che nel trifase $P_{cc} = 3R_{1cc}I_{1n}^2 = 3R_{2cc}I_{2n}^2$ allora...  

$R_{1cc} = \dfrac{P_{cc}}{3I_{1n}^2} = \dfrac{625}{3\cdot 1.44} \simeq 100.5\ \Omega$  

$R_{2cc} = \dfrac{P_{cc}}{3I_{2n}^2} = \dfrac{625}{3\cdot 36.08} \simeq 0.16\ \Omega$  

$X_{1cc} = R_{1cc}\tan\varphi_{cc} = 100.5\cdot 2.16 = 217.08\ \Omega$  

$X_{2cc} = R_{2cc}\tan\varphi_{cc} = 0.16\cdot 2.16 = 0.346\ \Omega$  

## 1 - Parametri trasversali  

```math
P_0 = \dfrac{P_{0\%}\cdot S_n}{100} \dfrac{1.5\cdot 25\ 000}{100} = 375\ W
```

$G_0 = \dfrac{P_0}{V_{1n}^2} = \dfrac{375}{10\ 000^2} \simeq 3.75\ \mu S$  

$B_0 = \dfrac{Q_0}{V_{1n}^2} = \dfrac{P_0\cdot\tan\varphi_0}{V_{1n}^2} = \dfrac{375\cdot 3.87}{10\ 000} \simeq 14.5\ \mu S$  

$G_0^{''} = G_0\cdot K_0^2 = 3.75\cdot 10^{-6}\cdot 25^2 \simeq 2.34\ mS$  

$B_0^{''} = B_0\cdot K_0^2 = 14.5\cdot 10^{-6}\cdot 25^2 \simeq 9.06\ mS$  

## 2 - Caduta di tensione e tensione sul carico  

Per la frazione di carico sappiamo che...  

$I_2 = \alpha\cdot I_{2n} = \dfrac{4}{5}\cdot 36.08 = 28.864\ A$  

Per cui...  

$\Delta V = \sqrt{3}\cdot I_2\bigg(R_{2cc}\cos\varphi_2+X_{2cc}\sin\varphi_2\bigg) = \sqrt{3}\cdot 28.864\bigg(0.16\cdot 0.8+0.346\cdot0.6\bigg) \simeq 16.78\ V$  

```math
\Delta V\% = \dfrac{\Delta V \cdot 100}{V_{20n}} = \dfrac{16.78\cdot 100}{400} = 4.195\ \%
```

$V_2 = V_{20n} - \Delta V = 400 - 16.78 = 383.22\ V$  

## 3 - Potenza attiva consumata dal carico e il rendimento  

$P_2 = \sqrt{3}\cdot V_2\cdot I_2\cdot \cos\varphi_2 = \sqrt{3}\cdot 383.22\cdot 28.864 \cdot 0.8 \simeq 15.33\ kW$  

$P_f = P_0\bigg(\dfrac{V_{1}}{V_{1n}}\bigg)^2 = 375\cdot\bigg(\dfrac{10\ 000}{10\ 000}\bigg)^2 = 375\ W$  

$P_{cu} = P_{cc}\bigg(\dfrac{I_2}{I_{2n}}\bigg)^2 = 625\cdot\bigg(\dfrac{28.864}{36.08}\bigg)^2 = 400\ W$  

```math
\eta = \dfrac{P_2}{P_1} = \dfrac{P_2}{P_2+P_f+P_{cu}} = \dfrac{15\ 330}{15\ 330+375+400} = \dfrac{15\ 330}{16105}\simeq 0.952 \implies \eta_{\%} = 95.2\ \%
```

## 4 - Impedenza delle fasi del carico  

In un carico collegato a triangolo sappiamo che $V = V_f$ per cui...  

$S_2 = Z_2\cdot I_2^2 \implies Z_2 = \dfrac{S_2}{I_2^2}$  

$S_2 = \dfrac{P_2}{\cos\varphi_2} = \dfrac{15.33}{0.8} \simeq 19.163\ kVA$  

$Z_2 = \dfrac{S_2}{I_2^2} = \dfrac{19\ 163}{28.864^2} \simeq 23\ \Omega$  

