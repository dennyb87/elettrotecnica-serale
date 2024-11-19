# Stabilita' dei sistemi  

Si vuole scoprire in che modo i poli di un sistema ne determinano la stabilita'. Consideriamo la seguente funzione di trasferimento:  

$G(s) = \dfrac{2}{s-10}+\dfrac{2}{s+10} = \dfrac{4s}{s^2-100}$  

Scopriamo che i poli sono...  

$s^2-100 = 0 \implies s = \sqrt{100}$  

$s_{P_1} = -10$  
$s_{P_2} = +10$  

Per semplicita' esaminiamo la risposta all'impulso $X(s) = 1$  

$Y(s) = G(s)\cdot X(s) = G(s)$  

$Y(s) \implies y(t) = 2e^{+10t}u(t)+2e^{-10t}u(t)$  

![system_stability](https://github.com/user-attachments/assets/2b2e3e6b-ccb2-4d12-bbea-42a39025efe1)  

Mentre il secondo termine $2e^{-10t}u(t)$ (in blu) e' transitorio in quanto tende a zero, il primo (in verde) cresce in modo esponenziale. Questo sistema risponde all'impulso con un segnale in uscita che non si stabilizza mai, e che realisticamente porterebbe al malfunzionamento del sistema se non la completa distruzione dello stesso.  

Si ha allora che un sistema e' stabile se i suoi poli sono negativi!  
