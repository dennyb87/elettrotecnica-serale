# Triangolo delle tensioni  

![circuito_RL_serie](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/05181fa8-470f-48d4-a78d-ba1a64c7aed5)  

Si vuole risolvere il circuito sapendo che:  

$E = \dfrac{E_{max}}{\sqrt{2}} \simeq 200\ V$  
$f = 10\ Hz$  
$R = 30\ \Omega$  
$L = 636.6\ mH$  
$X_L = \omega f = 2\pi fL \simeq 40\ \Omega$  

Troviamo l'angolo di sfasamento...  

$\varphi = \tan^{-1}(\frac{40}{30}) \simeq 53.13^\circ$  
$\cos \varphi = 0.6$  
$\sin \varphi = 0.8$  

Risolviamo allora il triangolo dell'impedenza con la relativa formula trigonometrica...  

$Z_{tot} = \dfrac{R}{\cos \varphi} = 50\ \Omega$  

Troviamo la corrente efficace con la legge di Ohm...  

$I = \dfrac{E}{Z_{tot}} = \dfrac{200}{50} = 4\ A$  

Risolviamo allora il triangolo delle potenze...  

$S = EI = 200 \cdot 4 = 800\ VA$  
$P = S \cdot \cos \varphi = 800 \cdot 0.6 = 480\ W$  
$Q = S \cdot \cos \varphi = 800 \cdot 0.8 = 640\ VAR$  

Si vuole ora risolvere il triangolo delle tensioni sapendo che la seconda legge di Kirchhoff e' sempre valida.  

$\vec{E} = \vec{V_R} + \vec{V_L}$  

$\vec{V_R} = R \cdot I = 30 \cdot 4 = 120\ V$  
$\vec{V_L} = jX_L \cdot I = j40 \cdot 4 = j160\ V$  

L'utilizzo della componente immaginaria in $jX_L$ rappresenta proprio lo sfasamento tra tensione e corrente nel componente, ovvero la tensione massima sui componenti non viene raggiunta nello stesso momento, per cui si ha infine che...  

$V = \sqrt{V_R^2+V_L^2} = \sqrt{120^2+160^2} = 200\ V$  
