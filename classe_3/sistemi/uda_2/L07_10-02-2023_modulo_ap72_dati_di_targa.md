# Modulo AP72  

Analizziamo ora i dati di targa del **modulo fotovoltaico AP72**.  

![modulo_ap72](https://user-images.githubusercontent.com/7195133/218302195-29262751-5ac3-42b5-a6d5-6ba4f107fb88.jpg)  

I dati di targa sono i dati di funzionamento, e si riferiscono alle prestazioni del modulo in condizioni standard (**STC** standard conditions). Esistono varie versioni del pannello con potenze di picco $W_p$ diverse, prendiamo in considerazione il modulo con potenza massima $260\ W_p$ ovvero **AP 72-260**.  

![modulo_ap72_dati_di_targa](https://user-images.githubusercontent.com/7195133/218302358-22ba43ab-bf92-4fd4-8c38-640251ecf4df.jpg)  


Notiamo prima di tutto che l'irraggiamento solare in condizioni standard e' di $1000\ W/m^2$ ad una temperatura di $25\degree C$ e un coefficiente di massa d'aria di $AM\ 1.5$  

## Coefficiente di massa d'aria  

Questo rappresenta il rapporto tra la lunghezza del percorso della radiazione solare attraverso l'atmosfera terrestre $L$ e il percorso che farebbe quando il sole e' allo zenith $L_z$ ovvero normale alla superficie terrestre. Si usa per caratterizzare le prestanzioni delle celle solari in condizioni standard il cui coefficiente e generalmente $1.5$.  

$AM = \dfrac{L}{L_z} = \dfrac{1}{\cos\theta} = 1.5$  

Questo equivale quindi ad un angolo di gradi $\cos^{-1}\frac{2}{3} \simeq 48.2\degree$  

![air_mass_coefficient](https://user-images.githubusercontent.com/7195133/218305317-dafdc0be-6a1a-4f1b-b969-42c694801652.jpg)  

## Rendimento  

Conoscendo la potenza radiante fornita dal sole $1000\ W/m^2$ possiamo ora calcolare il rendimento grazie alle misure del modulo $2 \times 1\ m$ che equivale ad un' area di $A = 2\ m^2$  

$P_{sun} = 1000\ \frac{W}{\cancel{m^2}} \cdot 2\ \cancel{m^2} = 2000\ W$  

Sapendo che il modulo ha una potenza massima di $260\ W_p$ possiamo allora calcolare il rendimento.  

$\eta = \dfrac{260}{2000} = 0.13$  

Questo coincide in effetti approssimativamente con i dati di targa $0.13 \simeq 13.3\ \%$  