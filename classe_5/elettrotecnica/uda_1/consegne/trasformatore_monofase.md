# Trasformatore monofase  

## Esercizio 1  

Si vuole determinare i parametri del circuito equivalente riportati al primario e al secondario di un trasformatore monofase avente i seguenti dati di targa:

```math
\begin{aligned}
    V_{1n} &= 400\ V\\
    V_{20n} &= 24\ V\\
    I_0 &= 1\ A\ \text{( lato 400 V)}\\
    \cos\varphi_0 &= 0.25\\
    R_1 &= 2\ \Omega\\
    X_1 &= 3\ \Omega\\
    R_2 &= 3\ m\Omega\\
    X_2 &= 5\ m\Omega\\
\end{aligned}
```

Troviamo il rapporto di trasformazione...  

$K_0 = \dfrac{V_{1n}}{V_{20n}} = \dfrac{400}{24} \simeq 16.67$  


#### Parametri longitudinali al primario  

$R_{1cc} = R_1 + R_2^\prime = R_1 + R_2 \cdot K_0^2 = 2 + 3\cdot 10^{-3} \cdot 16.67^2 \simeq 2.83\ \Omega$  

$X_{1cc} = X_1 + X_2^\prime = X_1 + X_2 \cdot K_0^2 = 3 + 5\cdot 10^{-3} \cdot 16.67^2 \simeq 4.39\ \Omega$  

#### Parametri longitudinali al secondario

$R_{2cc} = R_2 + R_1^{''} = R_2 + R_1 \cdot \dfrac{1}{K_0^2} = 3\cdot 10^{-3} + 2 \cdot \dfrac{1}{16.67^2} \simeq 10\ m\Omega$  

$X_{2cc} = X_2 + X_1^{''} = X_2 + X_1 \cdot K_0^2 = 5\cdot 10^{-3} + 3 \cdot \dfrac{1}{16.67^2} \simeq 15.8\ m\Omega$  

#### Parametri trasversali al primario  

$P_0 = V_{1n}\cdot I_0\cdot\cos\varphi_0 = 400\cdot 1 \cdot 0.25 = 100\ W$  

$G_0 = \dfrac{P_0}{V_{1n}^2} = \dfrac{100}{400^2} = 625\mu S$  

$\varphi_0 = \arccos 0.25 \simeq 75.522^\circ$  

$B_0 = G_0 \cdot \tan \varphi = 625\cdot10^{-6}\cdot\tan 75.522 \simeq 2.42\ mS$  

#### Parametri trasversali al secondario  

$G_0^{''} = G_0 \cdot K_0 = 625\cdot 10^{-6}\cdot 16.67^2 \simeq 174\ mS$  

$B_0^{''} = B_0 \cdot K_0 = 2.42\cdot 10^{-3} \cdot 16.67^2 \simeq 672\ mS$  

## Esercizio 2  

Determinare i parametri del circuito equivalente riferiti sia al primario, sia al secondario, di un trasformatoremonofase avente le seguenti caratteristiche:

```math
\begin{aligned}
    f_n &= 50\ Hz\\
    S_n &= 8000\ VA\\
    V_{1n} &= 500\ V\\
    V_{20n} &= 48\ V\\
    V_{cc\%} &= 6\ \%\\
    P_{cc\%} &= 3.2\ \%\\
    P_{0n\%} &= 1.5\ \%\\
    \cos\varphi_{0n} &= 0.22\\
\end{aligned}
```

#### Parametri longitudinali al primario  

$P_{cc} = \dfrac{P_{cc\%}\cdot S_n}{100} = \dfrac{3.2\cdot 8000}{100}= 256\ W$  

$I_{1n} = \dfrac{S_n}{V_{1n}} = \dfrac{8000}{500} = 16\ A$  

$R_{1cc} = \dfrac{P_{cc}}{I_{1n}^2} = \dfrac{256}{16^2} = 1\ \Omega$  

$\cos \varphi = \dfrac{P_{cc\%}}{V_{cc\%}} = \dfrac{3.2}{6} \simeq 0.533$  

$\varphi = \arccos 0.533 \simeq 57.79^\circ$  

$X_{1cc} = R_{1cc}\cdot\tan\varphi = 1 \cdot \tan 57.79 = 1.587\ \Omega$  

#### Parametri longitudinali al secondario  

$I_{2n} = \dfrac{S_n}{V_{20n}} = \dfrac{8000}{48} = 166.\overline{6}\ A$  

$R_{2cc} = \dfrac{P_{cc}}{I_{2n}^2} = \dfrac{256}{166.\overline{6}} = 9.216\ m\Omega$  

$X_{2cc} = R_{2cc}\cdot\tan\varphi = 9.216\cdot 10^{-3} \cdot \tan 57.79 \simeq\ 14.63\ m\Omega$  

#### Parametri trasversali al primario  

$P_0 = \dfrac{P_{0n\%}\cdot S_n}{100} = \dfrac{1.5\cdot 8000}{100} = 120\ W$  

$G_0 = \dfrac{P_0}{V_{1n}^2} = \dfrac{120}{500^2} = 625\mu S = 0.48\ mS$  

$\varphi_{0n} = \arccos 0.22 \simeq 77.29^\circ$  

$B_0 = G_0 \cdot \tan \varphi = 0.48\cdot10^{-3}\cdot\tan 77.29 \simeq 2.13\ mS$  

#### Parametri trasversali al secondario  

$K_0 = \dfrac{V_{1n}}{V_{20n}} = \dfrac{500}{48} \simeq 10.42$  

$G_0^{''} = G_0 \cdot K_0 = 0.48\cdot 10^{-3}\cdot 10.42^2 \simeq 52.12\ mS$  

$B_0^{''} = B_0 \cdot K_0 = 2.13\cdot 10^{-3} \cdot 10.42^2 \simeq 231.27\ mS$  


## Esercizio 3  

Considerando che il trasformatore dell'esercizio precedente venga alimentato da una rete primaria alla tensione di $500\ V$ ed alimenti un utilizzatore ohmico-induttivo che assorbe la corrente $I_2 = 120\ A$ con fattore di potenza $\cos\varphi_2 = 0.84$ determinare:
* la caduta di tensione, assoluta e percentuale
* il rendimento

```math
\Delta V = V_{20n} - V_2 = I_2\bigg(R_{2cc}\cos\varphi_2+X_{2cc}\sin\varphi_2\bigg) = 120\bigg(9.216\cdot 10^{-3}\cdot 0.84+14.63\cdot 10^{-3}\cdot 0.54\bigg) \simeq 1.88\ V
```

```math
\Delta V\% = \dfrac{\Delta V}{V_{20n}}\cdot 100 = \dfrac{1.88}{42}\cdot 100 \simeq 3.92\ \%
```

```math
P_0 = \dfrac{P_{0\%}\cdot S_n}{100} = \dfrac{1.5 \cdot 8000}{100} = 120\ W
```

$P_{cu} = R_{2cc}I_2^2 = 9.216\cdot 10^{-3} \cdot 120^2 \simeq 132.71\ W$  

$V_2 = V_{20n} - \Delta V = 48 - 1.88 = 46.12\ V$  

$P_2 = V_2I_2\cos\varphi_2 = 46.12\cdot 120\cdot 0.84 \simeq 4648\ W$  

$\eta = \dfrac{P_2}{P_2 +P_0+P_{cu}} = \dfrac{4648}{4648+120+132.71} \simeq 0.948$  

