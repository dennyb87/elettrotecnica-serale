# Alternatore  

Le **macchine sincrone** hanno diverse applicazioni tra cui quella del **generatore elettrico**, anche detto **alternatore**. A seconda della velocita' di rotazione necessaria il rotore viene realizzato in modi differenti:  

* **poli salienti** - basse velocita'
* **poli lisci** - alte velocita'


## Poli salienti  

![poli_salienti](https://github.com/user-attachments/assets/c7c71adf-c9c5-4621-8c7e-55c1357590c4)  


## Poli lisci  

![poli_lisci](https://github.com/user-attachments/assets/e35fca2f-7722-4ff7-83ff-d399f8d4ac9f)  

## Principio di funzionamento  

Nell'[alternatore](https://www.youtube.com/watch?v=tiKH48EMgKE) il rotore viene ruotato meccanicamente grazie all'albero, gli avvoglimenti rotorici sono percorsi da una corrente che puo' essere fornita direttamente dal motore primo, oppure grazie ad un circuito di eccitazione esterno. La corrente nell'avvoglimento rotorico crea un campo magnetico statico, ma il rotore e' messo in movimento dal motore primo che lo fa ruotare creando cosi' una variazione di flusso negli avvolgimenti statorici inducendovi una corrente sincronizzata con la velocita' del rotore, da cui il nome **macchina sincrona**. Non essendoci scorrimento si ha che...  

$n_0 = n = \dfrac{60f}{P}$  

# Funzionamento a vuoto  

![funzionament_a_vuoto](https://github.com/user-attachments/assets/38a09100-f99a-488e-8c23-6055159c229a)  

La macchina fuziona a vuoto quando:  

1. il motore primo fa ruotare il rotore a velocita' $n_0 = \dfrac{60f}{P}$ che dipende dalla frequenza desiderata
2. negli avvolgimenti rotorici passa la corrente di eccitazione che puo' essere eventualmente regolata
3. le fasi dell'avvolgimento indotto statorico sono scollegate dalla rete

Il circuito, nel caso di un collegamento a stella, risulta allora il seguente:  

![alternatore_vuoto](https://github.com/user-attachments/assets/c664a178-0048-43d3-99e7-1d548d36b875)  

Dove la tensione di fase a vuoto e' $V_{0f} = E_0$ mentre quella concatenata e' $V_0 = \sqrt{3}E_0$ (se a triangolo la tensione di fase e quella concatenata coincidono). Il valore efficace comune della tensione indotta dal flusso a vuoto si indica con:

$E_0 = K_1\cdot N\cdot f\cdot \phi_0$

Dove $K_1$ e' un coefficiente che tiene conto del tipo di avvolgimento mentre $N$ e' il numero di avvolgimenti, $f$ la frequenza, e $\phi_0$ e' il flusso a vuoto.  

### Bilanciamento delle potenze  

Nel funzionamento a vuoto la corrente sulle fasi statoriche e' nulla percio' le uniche potenze in gioco sono:  

* perdite di eccitazione $P_e$ a meno che il sistema di eccitazione non sia esterno
* perdite per attrito e ventilazione $P_{av}$
* perdite nel ferro $P_f$ dovute al flusso magnetico a vuoto presenti principalmente nel circuito magnetico statorico

$P_0 = P_e + P_{av} + P_f$  

## Funzionamento a carico e reazione d'indotto  

Nel funzionamento a carico le correnti statoriche creano un *campo magnetico rotante trifase* di reazione $\phi_r$ anche detto **campo indotto**. Questo influisce sul campo magnetico di eccitazione del rotore $\phi_e$ dando vita al flusso risultante $\phi$ (flusso a carico). In particolare si puo' notare che la tensione indotta nel circuito statorico subisce una variazione, e questa variazione viene attribuita a una reattanza fittizia di reazione $X_r$  

> la **reazione d'indotto** e' allora l'insieme dei fenomeni che si verificano nel passaggio da funzionamento a vuoto a quello a carico a causa delle correnti statoriche

### Circuito puramente ohmico  

Ricordando che per la legge di *Faraday-Neumann-Lenz* la tensione indotta $\vec{E_0}$ e' $90^\circ$ in ritardo rispetto al flusso di eccitazione $\vec{\phi_e}$ quindi al passaggio della corrente statorica $\vec{I}$ si crea un flusso di reazione $\phi_r$ che sommato (ipotesi di linearita') a quello di eccitazione da vita al flusso a carico $\vec{\phi}$ e di conseguenza ad una tensione a carico $\vec{E}$ in ritardo di $90^\circ$ e maggiore di $\vec{E_0}$ dato che la tensione e' proporzionale flusso $\vec{E} \propto \vec{\phi}$ 

![armature_reaction_ohmic](https://github.com/user-attachments/assets/4fd1359b-cb72-43be-9bfd-155915b4c7e5)  

Le reazioni d'indotto nei circuiti **puramente induttivi** o **capacitivi** si manifestano in modi simili.  

### Puramente induttivo  

![armature_reaction_inductive](https://github.com/user-attachments/assets/0fc69a06-2ded-48a5-8709-8937abccad42)  

### Puraemente capacitivo  

![armature_reaction_capacitive](https://github.com/user-attachments/assets/1a9ab3a0-240e-4ca2-bf5b-d38c13d988a7)  


