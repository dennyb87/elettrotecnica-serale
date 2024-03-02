# Circuito nel dominio di Laplace  

![ohmico_capacitivo_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/26da28e8-bf99-4fa8-9a74-633ce463d607)  

La seconda legge di Kirchhoff ci dice che:  

$e(t) = v_R+v_C = Ri +v_C$  

Ma $i = \dfrac{\Delta q}{\Delta t} = C\dfrac{\Delta v_C}{\Delta t}$ per cui...    

$e(t) = RC\dfrac{\Delta v_C}{\Delta t} + v_c$  

Nel tentativo di risolvere il circuito nel dominio del tempo ci troviamo di fronte alle derivate per le quali non abbiamo ancora nessuno strumento a nostra disposizione. E' necessario allora passare al dominio della frequenza con le trasformate di Laplace, in particolare si puo' dimostrare che:  

$i(t) = C\dfrac{\Delta v_C}{\Delta t} \implies I(s) = CsV_C(s)$  

Per la legge di Ohm generalizzata si ha allora che la reattanza capacitiva e' uguale a...  

$X_C(s) = \dfrac{V_C(s)}{I(s)} =\dfrac{\cancel{V_C(s)}}{Cs\cancel{V_C(s)}} = \dfrac{1}{Cs}$  

Sempre per la legge di Ohm la corrente del circuito e' anche uguale a:  

$I(s) = \dfrac{E(s)}{R+X_C} = \dfrac{E(s)}{R+\frac{1}{Cs}}$  

