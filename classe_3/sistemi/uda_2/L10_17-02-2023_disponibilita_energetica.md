# Calcolo disponibilita' energetica 

Tracciamo il grafico della potenza di irraggiamento al metro quadro nel luogo di utenza per una potenziale installazione di un pannello fotovoltaico.  

![disponibilita_energetica](https://user-images.githubusercontent.com/7195133/219953759-cd042a0d-2345-4d49-98e3-5c734793deea.jpg)  

Osserviamo che cominciamo ad ottenere potenza utile intorno alle 8am, questa potenza cresce fino ad arrivare a $400\ W/m^2$ intorno a mezzogiorno restando piu' o meno costante fino alle 14pm, per poi tornare di nuovo a zero alle 18pm. Possiamo allora calcolare l'energia totale al metro quadro disponibile in queste 10 ore.  

Tenedo presente la formula per il calcolo dell'area di un trapezio $\dfrac{(a + b) \cdot h}{2}$ oppure notando che in effetti i due triangoli rettangoli sono uguali, potendo allora considerarli un unico grande rettangolo, possiamo calcolare l'energia totale giornaliera disponibile al metro quadro, in quella determinata posizione geografica e periodo dell'anno.  

$\dfrac{(a + b) \cdot h}{2} = \dfrac{(10 + 2)\cdot 400}{2} = 6 \cdot 4000 = 2400\ Wh/m^2 = 2.4\ kWh/m^2$  

Questo significa che nel luogo di utenza, in un determinato periodo dell'anno, sono disponibili $2.4\ kWh/m^2$ giornalieri. Allora con un pannello da $2\ m^2$ si potrebbero produrre circa $2 \cancel{m^2} \cdot 2400 \frac{Wh}{\cancel{m^2}} = 4800\ Wh$ al giorno.  