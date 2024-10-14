# Trasformatore ideale  

![ideal_transformer_01](https://github.com/user-attachments/assets/140bf2f8-d4a2-4f57-a110-f37689830c0f)  

Applicando una tensione sinusoidale sul circuito primario nascera' un flusso magnetico sempre sinusoidale.  

$\phi = \phi_{max} \sin (\omega t)$  

I due avvolgimenti saranno quindi soggetti ad un flusso concatenato $\phi_c$ in dipendenza del numero delle loro spire.  

$\phi_c = N \phi_{max} \sin (\omega t)$  

Per la legge di *Faraday-Neumann-Lenz* la tensione a cui gli avvolgimenti sono sottoposti dipende dalla variazione del flusso nel tempo.  

$v = L\dfrac{\Delta i}{\Delta t} = \dfrac{\Delta \phi_c}{\Delta t} = N\cdot\phi_{max} \cdot\omega\cdot\sin (\omega t -\dfrac{\pi}{2})$  

E' importante notare che le tensioni indotte hanno uno sfasamento di $90^\circ$ rispento al flusso dovuto alla dipendenza dalla sua variazione.  

Il valore efficace e' invece dato da:  

$V = \dfrac{N\phi_{max}\omega}{\sqrt{2}} = \dfrac{N\phi_{max}2\pi f}{\sqrt{2}} = \dfrac{2\pi}{\sqrt{2}} \cdot N\phi_{max}f \simeq 4.44 \cdot N\phi_{max}f$  

Il rapporto tra le due tensioni indotte da orgine al rapporto spire $K_N$  

$\dfrac{V_1}{V_2} = \dfrac{\cancel{4.44} \cdot N_1\ \cancel{\phi_{max}f}}{\cancel{4.44} \cdot N_2\ \cancel{\phi_{max}f}} = \dfrac{N_1}{N_2} = K_N$  
