# Caduta di tensione sulla linea  

## Monofase  

![real_line_model](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/fbb84bd9-b0f6-4574-960d-5a677e18c8fb)  

Il modello non ideale di una linea di trasmissione di energia monofase tiene conto, per la seconda legge di Ohm, della resistenza del conduttore $R_\ell$ e di una componente induttiva $X_\ell$ mentre la componente capacitiva essendo trascurabile viene ignorata.  

La formula per calcolare la caduta di tensione su una linea monofase e' allora:  

$\Delta V = 2 \cdot (R_\ell \cos \varphi + X_\ell \sin \varphi) \cdot I$  

Si noti che per la trigonometria $R_\ell \cos \varphi + X_\ell \sin \varphi = Z$ per cui...  

$\Delta V = 2ZI$  

## Trifase  

![three_phase_line_model](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c4c97cda-433b-4868-bc1f-079351788b1c)  

Nel caso di una linea trifase simmetrica ed equilibrata si hanno invece tre correnti sfasate di $120^\circ$ per cui...  

$\Delta V = \sqrt{3} \cdot (R_\ell \cos \varphi + X_\ell \sin \varphi) \cdot I$  

## Caduta di tensione percentuale  

Questa indica appunto la percentuale di tensione perduta, formalmente e' il rapporto tra la caduta di tensione e la tensione in ingresso:  

$\Delta V \% = \dfrac{\Delta V}{E} \cdot 100$  

