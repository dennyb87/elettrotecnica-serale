# Esercizi motore asincrono trifase  

## Esercizio 1  

Calcolare il **numero di poli** di un motore asincrono trifase di cui sono note, in condizioni di funzionamento sotto carico, le seguenti caratteristiche:  

```math
    s_\% = 3.5\ \%
```
$$
\begin{aligned}
    f_r &= 2.1\ Hz\\
    n_s &= 63\ \text{rpm}\\
\end{aligned}
$$

Sapendo che $n_s = n_0 - n$ allora...  

$s = \dfrac{n_s}{n_0}=\dfrac{n_0-n}{n_0} \implies 0.035 = \dfrac{63}{n_0} \implies n_0=\dfrac{63}{0.035} = 1800\ \text{rpm}$  

Considerato che...  

$f_r = sf \implies f = \dfrac{f_r}{s} = \dfrac{2.1}{0.035} = 60\ Hz$  

...e che...  

$n_0 = \dfrac{60f}{P} \implies P = \dfrac{60f}{n_0} = \dfrac{60\cdot60}{1800} \simeq 2\ \text{coppie polari}$  

$2P = 4\ poli$  

## Esercizio 2  

Facendo riferimento all'esercizio precedente riportare la velocita' del campo magnetico rotante e del rotore in rad/s.  

$w_0 = \dfrac{2\pi n_0}{60} = \dfrac{2\pi\cdot 1800}{60} \simeq 188.5\ \frac{rad}{s}$  

$n = n_0\cdot(1-s) = 1800\cdot(1-0.035) \simeq 1737\ \text{rpm}$  

$w = \dfrac{2\pi n}{60} = \dfrac{2\pi \cdot 1737}{60} \simeq 181.9\ \frac{rad}{s}$  

## Esercizio 3  

Un motore asincrono trifase a 8 poli, con rotore avvolto, e collegamento degli avvolgimenti a triangolo e' alimentato da una rete primaria alla tensione $V_1 = 380\ V$ con frequenza $f=50\ Hz$. Nel funzionamento sotto carico, con scorrimento percentuale 3.7% il motore presenta le
seguenti caratteristiche:  

$$
\begin{aligned}
    P_f &= 720\ W\\
    P_{av} &= 500\ W\\
    P_r &= 15\ kW\\
    P_{j1} &= \dfrac{P_{j2}}{3}\\
    \cos\varphi_1 &= 0.88\\
\end{aligned}
$$

Calcolare il rendimento $\eta$ del motore, la coppia trasmessa $C_T$ e la corrente assorbita $I_1$ dalla rete primaria di alimentazione nelle condizioni specificate di carico.  


#### Potenza trasmessa  

$P_{j2}=sP_T$  

$P_T=P_r+P_{av}+sP_T$  

$P_T-sP_T=P_r+P_{av}$  

$P_T(1-s)=P_r+P_{av}$  

$P_T = \dfrac{P_r+P_{av}}{1-s} = \dfrac{15\cdot10^3+500}{1-0.037} \simeq 16\ 095.53\ W$  

#### Potenza assorbita  

$P_{pj1} = \dfrac{sP_T}{3}$  

$P_{add} = \dfrac{5\cdot P_a}{100}$

$P_a = P_T+P_f+\dfrac{sP_T}{3}+P_{add}$  

$P_a - 0.005P_a = P_T+P_f+\dfrac{sP_T}{3}$  

$P_a = \dfrac{P_T+P_f+\dfrac{sP_T}{3}}{1-0.005} = \dfrac{16\ 095.53+720+198.51}{0.995} \simeq 17\ 099.54\ W$  

#### Rendimento  

$\eta = \dfrac{P_r}{P_a} = \dfrac{15\ 000}{17\ 099.54} \simeq 0.877$  

#### Corrente sulla rete primaria  

$P_a = \sqrt{3}V_1I_1\cos\varphi_1$  

$I_1 = \dfrac{P_a}{\sqrt{3}V_1\cos\varphi_1} = \dfrac{17\ 099.54}{\sqrt{3}\cdot 380\cdot 0.88} \simeq 29.52\ A$  

#### Coppia trasmessa  

$n_0 = \dfrac{60f}{P} = \dfrac{60\cdot50}{4} = 750\ \text{rpm}$  

$C_T =\dfrac{P_T}{\omega_0}=\dfrac{60P_T}{2\pi n_0}=\dfrac{60\cdot 16\ 095.53}{2\pi\cdot750} = 204.93\ Nm$  
