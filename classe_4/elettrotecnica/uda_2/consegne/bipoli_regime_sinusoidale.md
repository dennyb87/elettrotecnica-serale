# Bipoli ohmico-induttivi-capacitivi in regime sinusoidale  

## ES1 - Bipolo resistivo  

![bipolo-resistivo-circuito](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/6ccfb749-8008-4d56-9d69-3ce7d165c219)  

Un resistore di resistenza $20\ \Omega$ è alimentato da un generatore sinusoidale di valore massimo $200\ V$, frequenza $10\ Hz$, fase $90^\circ$.  

![bipolo-resistivo-graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b5acbdc8-cbd8-48a8-86a1-952fec8a1f89)  

![bipolo-resistivo-vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/954a975c-4bd3-46c4-953e-19ec56fbc183)  

$V = \dfrac{V_{max}}{\sqrt{2}} = \dfrac{200}{\sqrt{2}} \simeq 141.421\ V$  

$I = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{10}{\sqrt{2}} \simeq 7.071\ A$  

$S = V \cdot I = \dfrac{200 \cdot 10}{2} = 1000\ VA$  

In un circuito puramente resistivo non c'e' sfasamento tra tensione e corrente, ovvero $\alpha = 0^\circ$ per cui la potenza apparente $S$ coincide con la potenza attiva $P$  

$P = S \cdot \cos 0^\circ = S \cdot 1 = 1000\ W$  

$Q = S \cdot \sin 0^\circ = S \cdot 0 = 0\ VAR$  


## ES2 - Bipolo capacitivo  

![circuito-capacitivo](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/19d80e5f-8770-4562-8172-8f124697de59)  

Un condensatore di capacita' $200\ \mu F$ è alimentato da un generatore sinusoidale di valore efficace $V = 50\ V$, frequenza $80\ Hz$, fase $\alpha = 0^\circ$  

$X_c = \dfrac{1}{\omega \cdot C} = \dfrac{1}{2\pi f \cdot C} = \dfrac{1}{2\pi \cdot 80 \cdot 200 \cdot 10^{-6}} \simeq 9.947\ \Omega$  

$V_{max} = V \cdot \sqrt{2} = 50 \cdot \sqrt{2} \simeq 70.711\ V$  

$I_{max} = 2\pi f\cdot C \cdot V_{max} = 2\pi \cdot 80 \cdot 200 \cdot 10^{-6} \cdot 70.711 \simeq 7.109\ A$  

$I = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{7.109}{\sqrt{2}} \simeq 5.027$  

$S = V \cdot I = 50 \cdot 5.027 = 251.35\ VA$  

In un circuito puramente capacitivo, non c'e' componente resistiva per cui corrente e tensione sono in quadratura con la corrente in anticipo di $90^\circ$  

$P = S \cdot \cos 90^\circ = S \cdot 0 = 0\ W$  

$Q = S \cdot \sin 90^\circ = S \cdot 1 = 251.35\ VAR$  

![capacitive_vi_vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7dea6d2f-d3b2-4bba-af9d-e9529bae53e7)  
