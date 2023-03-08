# Flusso magnetico  

Il flusso magnetico $\phi$ e' definito come l'insieme delle linee di forza che attraversano una superficie $S$ ovvero:  

$\phi = B \cdot S \cdot \cos \alpha$  

La sua unita' di misura e' il weber $Wb$ ovvero tesla metro quadro $Tm^2$. La motivazione dietro l'uso del fattore $\cos \alpha$ sta nel fatto che l'angolo $\alpha$ tra la superficie e il campo di induzione determina proprio il numero di linee passanti da questa, come si intuisce in figura.  

![magnetic_flux_basic](https://user-images.githubusercontent.com/7195133/223795307-5168856c-6b23-41c3-a724-7a9364b5a916.jpg)  

Solitamente si prende come riferimento il versore $\vec{n}$ normale alla superficie, il cui verso e' scelto in modo arbitrario, e rende chiaro che il flusso puo' quindi essere **entrante** o **uscente** dalla superficie a seconda del sistema di riferimento scelto.  

Si puo' allora osservare che con un angolo di $90^{\circ}$ si ha un $\cos \alpha$ uguale a zero percio' il flusso sara nullo. Si avra' invece flusso massimo quando l'angolo e' zero ovvero quando $\vec{n}$ e $\vec{B}$ hanno la stessa direzione e verso. Con un angolo di $180^{\circ}$ ovvero quando $\vec{n}$ e $\vec{B}$ hanno la stessa direzione ma verso opposto, si ha un $\cos \alpha$ uguale a $-1$ risultando quindi in un flusso $\phi$ negativo.  

## Flusso in un solenoide  

![solenoid_flux_basic](https://user-images.githubusercontent.com/7195133/223855028-f1ad69c7-47fc-4c46-9404-ebf498f12403.jpg)   

Posto in aria un avvolgimento di lunghezza complessiva $\ell = 40\ cm = 0.4\ m$ con $N = 60$ spire di sezione quadra con superficie $S = 400\ cm^2$ in cui scorre una corrente $I = 10\ A$ si puo' sperimentare che la forza magnetizzante al centro del solenoide e' uguale a:  

$H = \dfrac{NI}{\ell} = \dfrac{60 \cdot 10}{0.4} = 1500\ A/m$  

Possiamo quindi ora trovare il campo di induzione magnetica sapendo che in aria la permeabilita' magnetica e' pressoche' uguale a quella del vuoto $\mu_r \simeq 1$ percio' possiamo ignorare $\mu_r$ e tenere conto soltanto della permeabilita' del vuoto.  

$B = \mu_0 \cdot H = 4\pi \cdot 10^{-7} \cdot 1500 \simeq 1.885\ \mu T$  

![magnetic_flux_solenoid](https://user-images.githubusercontent.com/7195133/223852896-02fbd8ee-53c8-411e-a538-47046ac9c746.jpg)  

Adesso sapendo che la sezione e' $S = 400\ cm^2 = 400 \cdot 10^{-4}\ m^2 = 0.04\ m^2$ e scelto il versore $\vec{n}$ della superficie concorde a $\vec{B}$ possiamo trovare il flusso magnetico attraverso la sezione del solenoide.  

$\phi = B \cdot S \cdot \cos \alpha = 1.885 \cdot 10^{-3} \cdot 0.04 \cdot 1 \simeq 75.4\ \mu Wb$  