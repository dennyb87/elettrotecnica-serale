# Illuminazione  

La luce puo' essere descritta come un onda che si propaga nello spazio attraverso il campo elettromagnetico, come le onde radio, raggi X etc.. Oltre agli ormai noti parametri ampiezza, frequenza e periodo, si vuole introdurre il concetto di **lunghezza d'onda** indicata con il simbolo $\lambda$ che e' la distanza tra due massimi (o minimi) di una funzione periodica. Ne segue che la **velocita' di propagazione** e' uguale a:  

$v = \lambda \cdot f$  

Ovvero la distanza percorsa da $n$ cicli in un secondo. La velocita' di propagazione delle onde elettromagnetiche nel vuoto e' di circa $300\ 000\ \frac{km}{s}$  

![light-wave](https://github.com/user-attachments/assets/1fc83982-c7d8-4587-9d87-8fbb49a98a64)  

L'occhio umano riesce a percepire lunghezze d'onda comprese tra $400$ e $800$ circa nanometri ($10^{-9}$), questo prende il nome di **spettro visible**.  

![spectrum](https://github.com/user-attachments/assets/bc2662e7-08cb-451b-88f1-cce587e1b495)  


## Flusso luminoso $\Phi$  

![eye_sensitivity](https://github.com/user-attachments/assets/bc138e56-d510-42af-b539-7ea593d97caf)  

Il flusso luminoso (unita' di misura **lumen** $lm$) rappresenta l'energia per unita' di tempo, ovvero potenza, che tiene in considerazione la sensibilita' dell'occhio umano alle diverse lunghezze d'onda. Una potenza di $1\ W$ sotto forma di radiazione visibile a $\lambda = 550\ nm$ equivale a $\Phi = 680\ lm$ mentre se emessa a $\lambda = 600\ nm$ allora si hanno $\Phi =420\ lm$. In Particolare l'occhio umano ha sensibilita' massima intorno al **giallo-verde** $\lambda = 555\ nm$.  

## Illuminamento $E$  

L'illuminamento di una superficie e' il rapporto tra il flusso luminoso sulla superficie e l'area della superficie stessa. La sua unita' di misura e' il $\text{lux}$.  

$E = \dfrac{\Phi}{S} \bigg[\dfrac{\text{lm}}{m^2} = \text{lx (lux)}\bigg]$  


## Intensita' luminosa $I$  

![unit_steradian](https://github.com/user-attachments/assets/9309e0b0-f4e6-4fed-b5ec-dff1dd74f26f)  

(*steradiante unitario*)  

Questa' e' la quantita' di luce inviata in una certa direzione da una sorgente luminosa. Per definizione, il rapporto tra il flusso luminoso emesso in un cono nella stessa direzione, e l'apertura (**steradianti** $\Omega$) del cono stesso. La sua unita' di misura e' la candela $\text{cd}$  

$\Omega = \dfrac{A}{r^2}$  

$I = \dfrac{\Phi}{\Omega}$  

## Curve fotometriche   

![curve_fotometriche](https://github.com/user-attachments/assets/259eb5b6-3c20-4473-80cd-94e36eca29f0)  

L'intensita' luminosa in genere non e' costante in tutte le direzioni. I costruttori forniscono quindi le curve fotometriche che indicano l'intensita' luminosa nelle varie direzioni rispetto alla verticale, con riferimento ad un dispositivo che emette $1000\ \text{lumen}$. I valori delle curve devono percio' essere moltiplicati per il flusso luminoso del dispositivo in esame e divisi per mille.  

Volendo ricavare l'intensita' luminosa del dispositivo in figura a un angolo di $\gamma = 45^\circ$ si nota che a questa angolazione si hanno circa $110\ \text{lm}$. Dato che il dispositivo ha un flusso luminoso di $400\ \text{lm}$ allora l'intensita' luminosa a $45^\circ$ e'...  

$I = 110 \cdot \dfrac{400}{1000} = 44\ \text{cd}$  

## Luminanza $L$  

![luminanza](https://github.com/user-attachments/assets/209d0cae-548d-47c8-8930-5a0f29fd9841)  

La luminanza e' il rapporto tra l'intensita' luminosa di una superficie in una certa direzione e l'area apparente della superficie in quella direzione. La sua unita' di misura e' candela su metro quadro $\dfrac{\text{cd}}{m^2}$  

## Efficienza luminosa  

Il rappporto tra il flusso luminoso emesso e la potenza elettrica assorbita. Parte della potenza elettrica in ingresso viene persa in radiazioni non visibili. L'efficienza e' indicata con $\eta\ [\frac{\text{lm}}{\text{W}}]$ e rappresenta il rendimento, anche se per effetto dell'unita' di misura del flusso, questa puo' assumere valori maggiori dell'unita'.  

