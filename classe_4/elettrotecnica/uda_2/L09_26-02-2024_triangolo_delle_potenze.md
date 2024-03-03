# Triangolo delle potenze  

![rc_schema_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/91a547e4-ab5a-4855-9cb7-04ad63ee6ebe)  

Si vuole calcolare la potenza in gioco del circuito RC, tracciando la tensione del generatore e la corrente si puo' intuire che la differenza di fase non sia un angolo noto.  

![rc_vi_graph_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/da1b4c6a-c8d6-4bfa-865e-3449056551fa)  

Osservando che all'istante zero $i(0) \simeq 4.75\ A$ mentre $I_{max} \simeq 6\ A$ e' possibile stimare l'angolo di sfasamento.  

$i(0) = I_{max} \cdot \sin(\omega t + \alpha)$  

$4.75 = 6 \cdot \sin(\omega 0 + \alpha)$  

$\sin(\alpha) = \dfrac{4.75}{6} \simeq 0.7916$  

$\alpha = \sin^{-1}(0.7916) \simeq 52.34^\circ$  

Per un calcolo piu accurato si procede trovando l'angolo $\alpha$ e l'impedenza totale $Z$ del circuito passando dalla reattanza $X_c$  

$X_c = \dfrac{1}{2\pi f C} = \dfrac{1}{2\pi \cdot 0.5 \cdot 0.08} \simeq 3.98\ \Omega$  

$\alpha = \tan^{-1}\dfrac{R}{X_c} = \tan^{-1}\dfrac{3.98}{3} \simeq 53^\circ$  

$\cos \alpha = \cos 53^\circ \simeq 0.6$  

Si ha infine che l'impedenza totale e'...  

$Z = \dfrac{R}{\cos \alpha} = \dfrac{3}{0.6} = 5\ \Omega$  

Scopriamo allora che la corrente massima $I_{max}$ e'...  

$I_{max} = \dfrac{V_{max}}{Z} = \dfrac{30}{5} = 6\ A$  

Si ha quindi che il prodotto dei valori efficaci di tensione e corrente e' la **potenza apparente**.  

$S = \dfrac{V_{max}}{\sqrt{2}} \cdot \dfrac{I_{max}}{\sqrt{2}} = \dfrac{V_{max} \cdot I_{max}}{2} = \dfrac{30 \cdot 6}{2} = 90\ VA$  

![power_triangle](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/5bdf876f-fefc-43a6-9f2c-4961a558194c)  

Prende il nome di **potenza apparente** $S$ in quanto contiene una componente detta **potenza reattiva** $Q$ causata appunto dalla reattanza, questa potenza viene scambiata ma non trasformata al contrario della **potenza attiva** $P$  

$P = S \cdot \cos \alpha = 90 \cdot 0.6 = 54\ W$  

$Q = S \cdot \sin \alpha = 90 \cdot 0.8 = 72\ VAR$  
