# Potenza dissipata  

```mermaid
flowchart LR
    gen["generatore"]--"RL XL"---mat
    gen--"RL XL"---mat
    gen--"RL XL"---mat
```

Considerando lo schema di collegamento di un motore asincrono trifase o **mat**,  si vuole calcolare la caduta di tensione e la potenza dissipata sulla linea conoscendo:  

$V_1 = 400\ V$  
$R_\ell = 0.4\ \Omega$  
$X_\ell = 0.3\ \Omega$  
$I = 15\ A$  
$\eta = 0.7$  
$\cos \varphi_{mat} = 0.8$  

Calcoliamo quindi la caduta di tensione e la percentuale...  

$\Delta V = \sqrt{3} \cdot (R_\ell \cos \varphi_{mat} + X_\ell \sin \varphi_{mat}) \cdot I = \sqrt{3} \cdot (0.4 \cdot 0.8 + 0.3 \cdot 0.6) \cdot 15 \simeq 13\ V$  

$\Delta V \% = \dfrac{\Delta V}{V_1} \cdot 100 = \dfrac{13}{400} \cdot 100 = 3.25\ \%$  

La normativa impone una caduta di tensione percentuale minore del $4\ \%$ per cui $3.25\ \%$ soddisfa le condizioni.  

### Potenza dissipata sulla linea  

La componente induttiva sappiamo che scambia energia senza dissiparla, per cui per calcolare la potenza dissipata $P_d$ si utilizza soltanto la componente resistiva.  

$P_{d1} = V_{R_\ell} \cdot I = R_\ell \cdot I^2 = 0.4 \cdot 15^2 = 90\ W$  

Considerato che $P_{d1} = P_{d2} = P_{d3}$ la potenza totale dissipata sulla linea e'...  

$P_d = 3P_{d1} = 3 \cdot 90 = 270\ W$  

