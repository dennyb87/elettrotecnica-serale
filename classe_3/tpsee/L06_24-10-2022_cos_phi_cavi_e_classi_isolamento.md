# Calcolo corrente di due lampade in alternata

Prendiamo in considerazione un circuito in alternata a $230V$ con due lampade da $100W$ ed un fattore di potenza di $0.9$.  
Calcoliamo la corrente che vi scorre con una lampada accesa.  
$P_1 = V \cdot I \cdot \cos \varphi$  
$I_1 = I_2 = \frac{P}{V \cdot \cos \varphi} = \frac{100W}{230V \cdot 0.9} = 0.48A$  
$I = I_1 + I_2 = 0.48A + 0.48A = 0.96A$  

Si capisce quindi che nel circuito scorrono due correnti diverse a seconda di quante lampade si accendono.  
Accendendo una lampada si avra' una corrente di $0.48A$ mentre $0.96A$ se le accendessimo entrambe.  

# Accenni sui cavi  
## Tensione nominale  

![fs17](https://user-images.githubusercontent.com/7195133/198819412-a273efd9-a132-4163-8e6d-71fb3f70dad5.jpg)  

Sui cavi e' indicata la tensione nominale, prendiamo ad esempio la tensione nominale in figura $450/750V$.  
I due valori sono rispettivamente $U_0/U$ , di seguito il loro significato.  

$U_0$ e' la tensione massima **cavo-terra**, ovvero la tensione massima che il singolo conduttore isolato puo' supportare  
rispetto ad un qualunque oggetto conduttivo a potenziale zero adiacente allo stesso.  
Ad esempio, se il cavo fosse poggiato su un materiale conduttore come il telaio di una lavatrice, e la tensione del cavo  
fosse maggiore di $U_0$, allora l'isolante del cavo non riuscira' piu' a fermare il flusso di cariche che riuscira'  
ad arrivare al telaio mettendolo in tensione, diventando quindi pericoloso.  

$U$ e' invece la tensione massima **cavo-cavo** ovvero la tensione massima che l'isolamento del cavo puo supportare  
rispetto ad un altro cavo isolato a stretto contatto.  

**Perche' allora alcuni cavi hanno $U_0 = U$ ?**  


# Classi di isolamento  

## Classe 0  

E' la classe dove la protezione si basa sull'isolamento principale, cioe' il normale isolamento tra conduttori e carcassa  
o altre masse metalliche dell'apparecchio.  
Non e' previsto dunque nessun conduttore di protezione (messa a terra) o protezioni di altro genere.  
L'uso di questi in connesione alla rete elettrica non e' piu consentito in Italia, in quanto un semplice guasto puo' causare la folgorazione.  

## Classe 1  

![messa_a_terra](https://user-images.githubusercontent.com/7195133/198837885-2bc20c28-806e-4bba-95d4-6f3057a5f598.jpg)  

Sono di classe 1 i dispositivi che utilizzano il conduttore di protezione (messa a terra).  

![cavo_di_protezione](https://user-images.githubusercontent.com/7195133/198837894-e5cecc35-744d-4f23-ba06-3e58f7abf216.jpg)  


## Classe 2  

![doppio_isolamento](https://user-images.githubusercontent.com/7195133/198837975-3c05dd38-1c5d-4b1e-b5d5-c0100dc3cb05.jpg)

Questi dispositivi sono costruiti in modo che le parti in tensione siano circondate da un doppio strato di materiale isolante (isolamento principale + isolamento supplementare).  










