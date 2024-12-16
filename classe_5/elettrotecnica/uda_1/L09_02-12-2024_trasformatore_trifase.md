# Trasformatore trifase  

![trasformatore_trifase](https://github.com/user-attachments/assets/e35a5a39-f139-42a3-a0a9-ce05d4f1ac7d)  

La risoluzione del trasformatore trifase e' pressoche' identica a quella del trasformatore monofase ad eccezione di qualche formula in cui dobbiamo tenere conto delle 3 linee o dello sfasamento $\sqrt{3}$.  

$P_{cc} = 3\cdot R_{1cc}\cdot I_{1n}^2 = 3\cdot R_{2cc}\cdot I_{2n}^2$  

$S_n = \sqrt{3}\cdot V_{1n}\cdot I_{1n} = \sqrt{3}\cdot V_{20n}\cdot I_{2n}$  

Sapendo che...    

```math
\cos\varphi_{cc} = \dfrac{P_{cc\%}}{V_{cc\%}} \implies V_{cc\%} = \dfrac{P_{cc\%}}{\cos\varphi_{cc}}
```

Possiamo trovare le tensioni in cortocircuito come...  

```math
V_{1cc} = \sqrt{3}\cdot Z_{1cc}\cdot I_{1n} = \dfrac{V_{cc\%}\cdot V_{1n}}{100}
```
```math
V_{2cc} = \sqrt{3}\cdot Z_{2cc}\cdot I_{2n} = \dfrac{V_{cc\%}\cdot V_{2n}}{100}
```

Per i parametri traversali e' possibile ricavere $P_0$ con...  

$P_0 = \sqrt{3}\cdot V_{1n}\cdot I_0 \cdot \cos\varphi_0$  

Mentre la conduttanza $G_0$ e la suscettanza $B_0$ restano invariati...  

$G_0 = \dfrac{P_0}{V_{1n}^2}$  

$B_0 = \dfrac{Q_0}{V_{1n}^2} = \dfrac{P_0\cdot \tan\varphi_0}{V_{1n}^2}$  

Per trovare $\Delta V$ basta tenere conto dello sfasamento...  

$\Delta V = \sqrt{3}\cdot I_2\bigg(R_{2cc}\cos\varphi_2+X_{2cc}\sin\varphi_2\bigg)$  

