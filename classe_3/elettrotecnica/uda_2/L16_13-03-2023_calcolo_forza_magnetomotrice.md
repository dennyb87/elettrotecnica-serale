# Calcolo della forza magnetomotrice in un circuito magnetico  

Prima di iniziare va precisato che in questi calcoli ignoreremo il flusso disperso $\phi_d$ in quanto e' di piccola entita' rispetto al flusso nel circuito magnetico $\phi_{cm}$. Quindi nonostante il flusso totale sia la somma di queste due componenti, si tiene conto soltanto del flusso nel circuito.  

$\phi_d \ll \phi_{cm} \implies \phi = \phi_d + \phi_{cm} \simeq \phi_{cm}$  

![magnetic_flux_leakage](https://user-images.githubusercontent.com/7195133/225937979-6dbf091e-835b-4cd5-ae2d-a9397d125bd4.jpg)  

Supponiamo ora di voler calcolare la forza magnetomotrice in un circuito di ferro fucinato di lunghezza $\ell = 60\ cm = 0.6\ m$ con sezione $S =10\ cm^2 = 10 \cdot 10^{-4}\ m^2 = 10^{-3}\ m^2$ e sapendo che e' presente un flusso $\phi = 0.5\ mWb = 0.5 \cdot 10^{-3}\ Wb$.  

Non potendo derivare $\mu_r$ dobbiamo trovare prima il campo di induzione ed utilizzarlo per trovare il valore di $\mu_r$ corrispondente da opportune tabelle.  

$B = \dfrac{\phi}{S} = \dfrac{0.5 \cdot \cancel{10^{-3}}}{\cancel{10^{-3}}} = 0.5\ T$  

![caratteristiche_magnetizzazione_materiali](https://user-images.githubusercontent.com/7195133/225950030-544522da-00be-4807-8273-111184a1a1c9.jpg)  

Scopriamo allora che $\mu_r$ per un campo di induzione di $0.5\ T$ e' uguale a $2840$. Utilizziamo allora questa nuova informazione per trovare la riluttanza $\mathcal{R}$ ed infine la forza magnetomotrice $\mathcal{F}$.  

$\mathcal{R} = \dfrac{1}{\mu_0 \cdot \mu_r} \cdot \dfrac{\ell}{S} = \dfrac{1}{4\pi \cdot 10^{-7} \cdot 2840} \cdot \dfrac{0.6}{10^{-3}} \simeq 1.68\ \cdot 10^5\ H^{-1}$  

$\mathcal{F} = \mathcal{R} \cdot \phi = 1.68\ \cdot 10^5 \cdot 0.5 \cdot 10^{-3} = 84\ A_s$  


## Riluttanza magnetica e resistenza elettrica  

E' interessante notare che la riluttanza magnetica $\mathcal{R}$ e la resistenza elettrica $R$ non solo sono simili concettualmente ma anche dal punto di vista matematico sono espresse in modo del tutto analogo.  

$R = \rho \cdot \dfrac{\ell}{S}$  

$\mathcal{R} = \dfrac{1}{\mu} \cdot \dfrac{\ell}{S}$  

Dove $\ell$ e' la lunghezza del conduttore o del circuito magnetico, $S$ la sezione, $\rho$ la resistivita' del materiale, $\mu$ la permeabilita' magnetica del materiale.  