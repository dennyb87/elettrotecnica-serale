# Calcolo resistenza impianto disperdente  

Esercizi svolti consultando il manuale a pagina **X-171** tabella **X.10.15**

## Dispersore cilindrico infisso a profondita'  

Si vuole calcolare la resistenza di un picchetto lungo $\ell = 2.5\ m$ di diametro $D = 50\ mm$ posto in un pozzetto a $h = 60\ cm$ di profondita', assumendo una resistivita' del terreno di $\rho_E = 300\ \Omega m$  

$R_E = \dfrac{1}{2}\bigg(1+\dfrac{\ell}{\ell+h}\bigg)\cdot\dfrac{\rho_E}{2\pi\ell}\cdot\ln \dfrac{2\ell}{a}$  

Dove $a$ e' il raggio del dispersore $a = \dfrac{D}{2} = \dfrac{50}{2} = 25\ mm$ per cui...  

$R_E = \dfrac{1}{2}\bigg(1+\dfrac{2.5}{2.5+0.6}\bigg)\cdot\dfrac{300}{2\pi\cdot2.5}\cdot\ln \bigg(\dfrac{2\cdot 2.5}{25\cdot 10^{-3}}\bigg) \simeq 91.4\ \Omega$  

## Dispersore cilindrico lineare  

Si ha una corda posata a $h = 0.6\ m$ di profondita' su tre lati di uno stabilimento lunga $\ell = 115\ m$ di area $A = 50\ mm^2$. Vogliamo calcolare la resistenza dell'impianto disperdente assumendo una resistivita' del terreno di $\rho_E = 250\ \Omega m$  

$R_e = \dfrac{\rho_E}{2\pi\ell}\bigg[\ln\bigg(\dfrac{2\ell}{a}\bigg)+\ln\bigg(\dfrac{\ell}{h}\bigg)-2+\dfrac{2h}{\ell}\bigg]$  

Dove $a$ e' il raggio del dispersore...  

$A = 50\ mm^2 = \pi a^2 \implies a = \sqrt{\dfrac{A}{\pi}} = \sqrt{\dfrac{50}{\pi}} \simeq 4\ mm$  

$R_E = \dfrac{250}{2\pi\cdot115}\bigg[\ln\bigg(\dfrac{2\cdot 115}{4\cdot 10^{-3}}\bigg)+\ln\bigg(\dfrac{115}{0.6}\bigg)-2+\dfrac{2\cdot 0.6}{115}\bigg] \simeq 4.92\ \Omega$  

## Dispersore ad anello  

Si ha una corda con sezione di area $A = 50\ mm^2$ lungo il perimetro di uno stabile $30\ m \times 15\ m$ posata a $h = 0.8\ m$ di profondita'. Si vuole calcolare la resistenza dell'impianto disperdente assumendo una resistivita' del terreno di $\rho_E = 100\ \Omega m$. La corda si richiude su se stessa, percio' utilizziamo la formula del dispersore ad anello trovando prima il perimetro $P$ e poi le misure del cerchio equivalente...  

$P = 2\cdot 30 + 2\cdot 15 = 90\ m$  

$P = 90\ m =2\pi r \implies r = \dfrac{P}{2\pi} = \dfrac{90}{2\pi} \simeq 14.32\ m$  

$A = 50\ mm^2 = \pi a^2 \implies a = \sqrt{\dfrac{A}{\pi}} = \sqrt{\dfrac{50}{\pi}} \simeq 4\ mm$  

Dove $r$ e' il raggio del cerchio equivalente formato dalla corda, mentre $a$ e' di nuovo il raggio della sezione della corda.  

$R_E = \dfrac{\rho_E}{4\pi^2r}\cdot\bigg[\ln\bigg(\dfrac{8r}{a}\bigg)+\ln\bigg(\dfrac{4r}{h}\bigg)\bigg] = \dfrac{100}{4\pi^2\cdot 14.32}\cdot\bigg[\ln\bigg(\dfrac{8\cdot 14.32}{4\cdot 10^{-3}}\bigg)+\ln\bigg(\dfrac{4\cdot 14.32}{0.8}\bigg)\bigg] \simeq 2.57\ \Omega$  

## Rete magliata  

Si vuole calcolare la resistenza dell'impianto di terra realizzato con una rete magliata di $50\ m\times 20\ m$ divisa in quadranti di $10\ m\times 10\ m$ ovvero con $3$ conduttori sul lato lungo, e $5$ sul lato corto. Assumendo una resistivita' del terreno di $\rho_E = 250\ \Omega m$ si vuole calcolare la resistenza del dispersore.  

$R_E = \dfrac{\rho_E}{4 r}+\dfrac{\rho_E}{\ell}$  

Dove $\ell$ e' la lunghezza totale del dispersore, ovvero:  

$\ell = 3\cdot 50 + 5\cdot 20 = 250\ m$  

Mentre $r$ e' il raggio del cerchio equivalente formata dalla maglia, quindi trovando il perimetro...  

$P = 2\cdot 20+2\cdot 50 = 140\ m$  

$P = 140\ m = 2\pi r \implies r = \dfrac{140}{2\pi}\simeq 22.28\ m$  

$R_E = \dfrac{250}{4\cdot 22.28} + \dfrac{250}{270}\simeq 3.73\ \Omega$  
