# Risolvere circuito trifase  

![three_phase_no_neutral](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/224af0c6-c4c0-421f-9625-43ebb5624068)  

Se il sistema trifase e' costituito da tre circuiti monofase ed il carico e' equilibrato, ovvero se i vettori delle impedenze coincidono, allora per risolverlo e' sufficiente risolvere uno dei circuiti monofase.  

![solve_single_phase_circuit](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f0a2f670-86d0-49fe-ae21-74b2cef0f6b7)  

Troviamo la reattanza dell'induttore $X_L$ e l'angolo di sfasamento $\varphi$ tra tensione e corrente...  

$X_L = L \omega = L 2 \pi f = 0.019 \cdot 2 \cdot \pi \cdot 50 \simeq 6\ \Omega$  

$\varphi = \tan^{-1} \frac{X_L}{R} = \tan^{-1} \frac{6}{8} \simeq 36.87^\circ$  

$\cos \varphi \simeq 0.8$  
$\sin \varphi \simeq 0.6$  

Troviamo quindi l'impedenza e la corrente...  

$Z = \dfrac{R}{\cos \varphi} = \dfrac{8}{0.8} = 10$  

$I = \dfrac{E_1}{Z} = \dfrac{230}{10} = 23\ A$  

![inductor_load_vectors](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9418a1b8-5d98-4086-98a1-a9e65874c269)  

Essendo un carico ohmico-induttivo le correnti sono in ritardo rispetto alle tensioni, in particolare con angolo $\varphi = 36.87^\circ$. A questo punto non resta che trovare le potenze:  

$S = VI = 230 \cdot 23 = 5290\ VA$  
$P = S \cdot \cos \varphi = 5290 \cdot 0.8 = 4232\ W$  
$Q = S \cdot \sin \varphi = 5290 \cdot 0.6 = 3174\ VAR$  

Ma i circuiti monofase sono identici percio' li abbiamo risolti tutti. Infine per trovare le potenze totali e' sufficiente ricorrere al teorema di *Boucherot*.  

$P_{tot} = P_1 + P_2 + P_3 = 3P = 4232 \cdot 3 = 12696\ W$  
$Q_{tot} = Q_1 + Q_2 + Q_3 = 3Q = 3174 \cdot 3 = 9522\ VAR$  
$S_{tot} = \sqrt{P_{tot}^2+Q_{tot}^2} = \sqrt{12696^2+9522^2} = 15870\ VA$  

Per un carico equilibrato si ha che...  

$S_{tot} = \sqrt{P_{tot}^2+Q_{tot}^2} = 3S$  

