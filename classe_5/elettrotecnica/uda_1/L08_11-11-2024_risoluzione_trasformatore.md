# Risoluzione del trasformatore  

![transformer-2nd](https://github.com/user-attachments/assets/7921de1b-d5fa-4791-a317-07bb268e5f54)  

Dato un trasformatore con le seguenti caratteristiche:  

```math
\begin{aligned}
    S_n &= 10\ kVA\\
    V_{1n} &= 3000\ V\\
    V_{2n} &= 250\ V\\
    P_{cc\%} &= 2.5\ \%\\
    P_{0\%} &= 1.5\ \%\\
    \cos \varphi_{cc} &= 0.5\\
    \cos \varphi_0 &= 0.35\\
\end{aligned}
```

Lo si alimenta con una tensione $V_1 = 2900\ V$ conoscendo il fattore di potenza nella nuova configurazione $\cos \varphi_2 = 0.85$ e la funzione di carico, ovvero il rapporto tra la corrente nel circuito e quella nominale.  

$\alpha = \dfrac{I_2}{I_{2n}} = \dfrac{4}{5}$  

Si vuole quindi trovare il valore di **tensione** sul carico, **perdite nel rame**, **perdite nel ferro**, **corrente** di esercizio, e **corrente di cortocircuito** in caso di guasto.  

## Tensione sul carico  

Per trovare $V_2$ vogliamo lavorare sul secondario portandovi tutti i parametri longitudinali come in figura, si ha allora che...  

$V_2 = V_{20} - \Delta V$  

$\Delta V = I_2\bigg(R_{2cc}\cos\varphi_2 + X_{2cc}\sin\varphi_2\bigg)$  

#### Tensione sull'avvolgimento  

Ricaviamo $V_{20}$ grazie al rapporto di trasformazione...  

$K_0 = \dfrac{V_{1n}}{V_{2n}} = \dfrac{3000}{250} = 12$  

$V_{20} = V_1 \cdot \dfrac{1}{K_0} = \dfrac{2900}{12} \simeq 241.67\ V$  

### Corrente  

Per trovare $I_2$ sfruttiamo la funzione di carico...  

$I_{2n} = \dfrac{S_n}{V_{2n}} = \dfrac{10\ 000}{250} = 40\ A$  

$I_2 = I_{2n}\cdot \dfrac{4}{5} = 32\ A$  

### Resistenza  

Adesso non resta che trovare $R_{2cc}$ sapendo che le perdite in cortocircuito $P_{cc}$ sono uguali alle perdite nel rame $P_{cu}$ in condizioni nominali, ovvero...  

$P_{cc} \simeq P_{cu} = R_{1cc}I_{1n}^2 = R_{2cc}I_{2n}^2$  

Troviamo le perdite in cortocircuito...  

```math
P_{cc} = S_n \cdot \dfrac{P_{cc\%}}{100} = 10\ 000\cdot\dfrac{2.5}{100} = 250\ W
```

Dalle perdite ricaviamo $R_{2cc}$  

$R_{2cc} = \dfrac{P_{cc}}{I_{2n}^2} = \dfrac{250}{40^2} \simeq 0.156\ \Omega$  

