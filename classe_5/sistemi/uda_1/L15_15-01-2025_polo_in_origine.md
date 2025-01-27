# Sistema con polo nell'origine  

In questo sistema la funzione di trasferimento nella forma $\dfrac{N(s)}{D(s)}$ ha il denominatore che si annulla con un valore di $s$ uguale a zero.  

$G(s) = \dfrac{1}{s} \implies G(j\omega) = \dfrac{1}{j\omega}$  

$G(j\omega)=\dfrac{1}{j\omega}\cdot\dfrac{j}{j}=\dfrac{j}{j^2\omega}=\dfrac{j}{-\omega}= -j\dfrac{1}{\omega}$  

Ne segue che...  

$|G| = -\dfrac{1}{\omega}$  

$\angle G = -90^\circ$  

Il grafico lineare del modulo di $G$ sara' allora di questo tipo...  

![filtro_integratore_lineare](https://github.com/user-attachments/assets/3b087d7a-1a63-475e-a50c-6f0f106bae04)  

Mentre per il diagramma di Bode troviamo $|G|_{dB}$  

$|G|_{dB} = 20\log \frac{1}{\omega} = 20\log \omega^{-1} = 20 -\log\omega = -20\log\omega$  

Percio' il grafico presentera' una retta con pendenza $-20\ \frac{dB}{\text{dec}}$  

![bode_filtro_integratore](https://github.com/user-attachments/assets/078b580e-51a1-42e8-b0be-10f8e3ddf365)  

