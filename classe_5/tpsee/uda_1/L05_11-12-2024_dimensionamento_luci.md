# Dimensionamento luci  

![mensa](https://github.com/user-attachments/assets/d91236b0-1377-47f2-bf6a-a43ea6c06602)  

Si vuole dimensionare l'illuminazione di una locale con le seguenti caratteristiche:

* il locale e' adibito a **mensa scolastica** 
* pareti e soffitto di colore **bianco**
* lampade installate al soffitto $\Phi = 2800\ lm$
* altezza locale $H = 4\ m$
* area $a \cdot b = 10 \cdot 30 = 300\ m$

Per prima cosa consultiamo il manuale a pagina **XI-54/58** per trovare l'illuminamento minimo richiesto per questo tipo di locali. Scopriamo che per le mense scolastiche sono richiesti:  

* illuminamento minimo $E_m = 200\ \text{lux}$  
* resa cromatica $R_a \ge 80$
* indice di abbagliamento limite (*Unified Glare Rating*) $U_{GR_L} \le 22$

## Metodo del flusso totale  

Questo metodo permette di calcolare il numero di corpi illuminanti $N$ necessari a soddisfare le condizioni:  

$N = \dfrac{E_m\cdot a\cdot b}{\Phi\cdot\mu\cdot M_f}$  

Dove $a\cdot b$ e' la superficie del locale in metri, $\mu$ e' il coefficiente di utilizzazione, $M_f$ e' il fattore di manutenzione generalment uguale a $0.8$.  

### Coefficiente di utilizzazione  

![utilisation_factor_table](https://github.com/user-attachments/assets/4e59c545-1ee1-4953-92db-29591bb5e4a2)  

Per determinare $\mu$ dobbiamo prima calcolare il coefficiente di riflessione $K$ con la formula:  

$K = \dfrac{a\cdot b}{h\cdot(a+b)}$  

Dove $h$ e' la distanza tra la superficie da illuminare e il corpo illuminante. Nel nostro caso assumiamo che i tavoli della mensa siano alti un metro, per cui $h=H-1=4-1=3\ m$  


$K = \dfrac{10\cdot 30}{3\cdot(10+30)} = \dfrac{300}{120} = 2.5$  

Una volta trovato $K$ possiamo ricavare $\mu$ dalla tabella fornita dal costruttore della lampada. Trattandosi di pareti e soffitti bianchi, facciamo riferimento alla prima colonna, ovvero $\mu = 1.08$  

$N = \dfrac{E_m\cdot a\cdot b}{\Phi\cdot\mu\cdot M_f} = \dfrac{200\cdot 10\cdot 30}{2800\cdot 1.08\cdot 0.8} \simeq 24.8 \implies 25\ \text{lampade}$  

### Installazione corpi illuminanti  

![distribuzione_lampade](https://github.com/user-attachments/assets/b9bde1a4-d264-4eba-8639-fce1a98e31df)

Trovato il numero di lampade si vogliono calcolare le misure d'installazione. Si ipotizza di installare le lampade in una configurazione $25=5\times5$ per cui...  

$x = \dfrac{a}{5} = \dfrac{10}{5} = 2\ m$  

$y = \dfrac{b}{5} = \dfrac{30}{5} = 6\ m$  

Una condizione da rispettare e' che la distanza dalle pareti deve essere la meta' della distanza tra le lampade.  
