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
rispetto ad un altro cavo adiacente dello stesso tipo.  

![H03VVH2-F-300-300](https://user-images.githubusercontent.com/7195133/199588248-7e8f7e9c-d9d9-4534-93c6-ed470e749e64.jpg)  

Non mi e' ancora del tutto chiaro perche' cavi con piu' di un anima come il [H03VVH2-F 300/300 V](https://www.comcavi.it/cavi/cavi-elettrici-bassa-tensione/h03vvh2-f/) in figura abbiano $U_0 = U$.  
Una spiegazione potrebbe essere che la guaina venga considerata in questo caso come isolante, quindi tra le due anime si ha $U$, mentre tra una  
delle due, e il conduttore immaginario a contatto con la guaina si avrebbe $U_0$, che risulta quindi uguale a $U$ dato lo spessore della guaina.  

Comunque non sono il solo ad essere confuso, vedi [electronics.stackexchange](https://electronics.stackexchange.com/questions/640653/what-determines-the-voltage-rating-of-a-cable-and-why-do-some-cables-have-u-0).


# Classi di isolamento  


|classe|simbolo|descrizione|
|--|--|--|
|0||E' la classe dove la protezione si basa sull'isolamento principale, cioe' il normale isolamento tra conduttori e carcassa o altre masse metalliche dell'apparecchio. Non e' previsto dunque nessun conduttore di protezione (messa a terra) o protezioni di altro genere. L'uso di questi in connesione alla rete elettrica non e' piu consentito in Italia, in quanto un semplice guasto puo' causare la folgorazione.|
|1|![messa_a_terra](https://user-images.githubusercontent.com/7195133/198837885-2bc20c28-806e-4bba-95d4-6f3057a5f598.jpg)|Sono di classe 1 i dispositivi che utilizzano il conduttore di protezione (messa a terra).|
|2|![doppio_isolamento](https://user-images.githubusercontent.com/7195133/198837975-3c05dd38-1c5d-4b1e-b5d5-c0100dc3cb05.jpg)|Questi dispositivi sono costruiti in modo che le parti in tensione siano circondate da un doppio strato di materiale isolante (isolamento principale + isolamento supplementare).|
|3|![classe_terza_isolamento](https://user-images.githubusercontent.com/7195133/199117278-b9d5cc57-453a-4bc5-a14c-c8701d75e31f.jpg)|Questi apparecchi non devono essere provvisti di alcuna protezione in quanto sono alimentati da bassissime tensioni|

 

# Tipi di pose  

|tipo di posa|esempio|descrizione|
|--|--|--|
|a vista||La posa a vista consiste semplicemnte nel fissare il conduttore su di una superficie visibile e.g. fissato ad una parete.|
|interrata|![posa_interrata](https://user-images.githubusercontent.com/7195133/198840459-ffff4c79-fa79-476e-85df-fd50fe953fef.jpg)|Letteralmente sottoterra quindi dentro ad un corrugato o un qualche altro tipo di protezione meccanica.|
|controsoffitto|![posa_controsoffitto](https://user-images.githubusercontent.com/7195133/198839933-8b2a3ce6-cd3d-47dd-a272-26017934a537.jpg)||
|in canale|![canale](https://user-images.githubusercontent.com/7195133/198839821-b78243e2-e6b6-468c-b807-8baa70c32285.jpg)||
|in passerella asolata|![passerella_asolata](https://user-images.githubusercontent.com/7195133/198838960-c26f0e56-5ff6-4d25-ba03-c641d302dfce.jpg)||
|in passerella a filo|![passerella_a_filo](https://user-images.githubusercontent.com/7195133/198839026-4825edf1-3fc2-4f17-bd7b-0b8fbcfe305b.jpg)||


