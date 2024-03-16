# Bipoli ohmico-induttivi-capacitivi in regime sinusoidale  

## ES1 - Bipolo resistivo  

![bipolo-resistivo-circuito](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/6ccfb749-8008-4d56-9d69-3ce7d165c219)  

Un resistore di resistenza $20\ \Omega$ è alimentato da un generatore sinusoidale di valore massimo $200\ V$, frequenza $10\ Hz$, fase $90^\circ$.  

![resistive_vip_graph](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/5b12566e-a24e-490a-90a6-7a5e884d0071)


![bipolo-resistivo-vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/954a975c-4bd3-46c4-953e-19ec56fbc183)  

$V = \dfrac{V_{max}}{\sqrt{2}} = \dfrac{200}{\sqrt{2}} \simeq 141.421\ V$  

$I = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{10}{\sqrt{2}} \simeq 7.071\ A$  

$S = V \cdot I = \dfrac{200 \cdot 10}{2} = 1000\ VA$  

In un circuito puramente resistivo non c'e' sfasamento tra tensione e corrente, ovvero $\alpha = 0^\circ$ per cui la potenza apparente $S$ coincide con la potenza attiva $P$  

$P = S \cdot \cos 0^\circ = 1000 \cdot 1 = 1000\ W$  

$Q = S \cdot \sin 0^\circ = 1000 \cdot 0 = 0\ VAR$  


## ES2 - Bipolo capacitivo  

![circuito-capacitivo](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/19d80e5f-8770-4562-8172-8f124697de59)  

Un condensatore di capacita' $200\ \mu F$ è alimentato da un generatore sinusoidale di valore efficace $V = 50\ V$, frequenza $80\ Hz$, fase $\alpha = 0^\circ$  

$X_C = \dfrac{1}{\omega \cdot C} = \dfrac{1}{2\pi f \cdot C} = \dfrac{1}{2\pi \cdot 80 \cdot 200 \cdot 10^{-6}} \simeq 9.947\ \Omega$  

$V_{max} = V \cdot \sqrt{2} = 50 \cdot \sqrt{2} \simeq 70.711\ V$  

$I_{max} = 2\pi f\cdot C \cdot V_{max} = 2\pi \cdot 80 \cdot 200 \cdot 10^{-6} \cdot 70.711 \simeq 7.109\ A$  

Si noti che coincide con...  

$I_{max} = \dfrac{V_{max}}{X_C} = \dfrac{70.711}{9.947} \simeq 7.109\ A$  

$I = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{7.109}{\sqrt{2}} \simeq 5.027$  

$S = V \cdot I = 50 \cdot 5.027 = 251.35\ VA$  

In un circuito puramente capacitivo, non c'e' componente resistiva per cui corrente e tensione sono in quadratura con la **corrente in anticipo** rispetto alla tensione di $90^\circ$  

$P = S \cdot \cos 90^\circ = 251.35 \cdot 0 = 0\ W$  

$Q = S \cdot \sin 90^\circ = 251.35 \cdot 1 = 251.35\ VAR$  

![capacitive_vi_vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7dea6d2f-d3b2-4bba-af9d-e9529bae53e7)  


## ES3 - Bipolo induttivo  

![circuito-induttivo](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7d2f1cfa-113f-49b4-81c8-5b2fa04dd15a)  

Un induttore di induttanza $20\ mH$ e' alimentato da un generatore sinusoidale di valore efficace $100\
V$, frequenza $200\ Hz$, fase $0^\circ$  

$X_L = \omega L = 2\pi f \cdot L = 2\pi \cdot 200 \cdot 20 \cdot 10^{-3} \simeq 25.133\ \Omega$  

$V_{max} = V \cdot \sqrt{2} = 100 \cdot \sqrt{2} \simeq 141.421\ V$  

$I_{max} = \dfrac{V_{max}}{X_l} = \dfrac{141.421}{25.133} = 5.627\ A$  

$I = \dfrac{I_{max}}{\sqrt{2}} = \dfrac{5.627}{\sqrt{2}} \simeq 3.979\ A$  

$S = V \cdot I = 100 \cdot 3.979 = 397.9\ VA$  

In un circuito puramente induttivo, non c'e' componente resistiva per cui corrente e tensione sono in quadratura con la **corrente in ritardo** rispetto alla tensione di $90^\circ$  

$P = S \cdot \cos 90^\circ = 397.9 \cdot 0 = 0\ W$  

$Q = S \cdot \sin 90^\circ = 397.9 \cdot 1 = 397.9\ VAR$  

![inductive_vi_vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/09c37dd2-e2bb-4c12-b351-317a9ede85ee)  
