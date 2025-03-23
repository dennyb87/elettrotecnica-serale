# Circuito equivalente di Behn-Eschemburg  

Con le opportune ipotesi semplificative e' possibile utilizzare questo circuito equivalente per macchine a poli lisci funzionanti sul tratto lineare della caratteristica.  

![behn-eschemburg](https://github.com/user-attachments/assets/96bf72f8-ed2f-4d3c-9eb6-82ffcae87d38)  


Dove $X_d + X_r = X_s$ detta **reattanza sincrona**, mentre $R_i+jX_s = \vec{Z_s}$ detta **impedenza sincrona**. Il valore di $Z_s$ puo' essere ricavato grazie alla corrente di cortocircuito (bypassando il carico)...  

$Z_s = \dfrac{E_0}{I_{cc}}$  

Dal circuito infine si ricava...  

$E_0^2 = \bigg(V_f\cdot\cos\varphi+R_iI\bigg)^2+\bigg(V_f\cdot\sin\varphi+X_sI\bigg)^2$  

## Bilancio delle potenze  

![potenze_circuito_equivalente](https://github.com/user-attachments/assets/3707a4a4-c26e-4a97-b889-197ef01c3851)  

Si hanno allora:  

* potenziali perdite di eccitazione $P_e = I_e\cdot V_e$
* perdite di attrito e ventilazione $P_{av}$
* perdite nel ferro $P_f$
* perdite nel rame statorico $P_{j1} = 3R_iI^2$
* perdite addizionali $P_{add}$

La potenza in uscita o potenza resa e' uguale a:  

$P = \sqrt{3}\cdot V\cdot I \cdot\cos\varphi$  

Dove $V$ e' la tensione concatenata, nella configurazione a stella $V = \sqrt{3}V_f$ mentre $I$ e' la corrente erogata. Alternativamente...  

$P = P_a-P_e-P_{av}-P_f-P_{j1}-P_{add}$  

Il rendimento e' dato da:  

$\eta = \dfrac{P}{P_a}$  

Si ricorda inoltre che per le perdite nel ferro vale la formula:  

$P_f = P_{fn}\bigg(\dfrac{V}{V_n}\bigg)^2$  
