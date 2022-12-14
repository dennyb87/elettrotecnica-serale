# Oscilloscopio  

![oscilloscopio](https://user-images.githubusercontent.com/7195133/195995150-602c58f5-290f-4ab6-a8f3-7159d3e07986.jpg)![oscilloscopio_divisioni](https://user-images.githubusercontent.com/7195133/195994724-435a73e8-163a-4487-8a97-890d9f3d81f5.jpg)  

L'oscilloscopio e' uno strumento che consente di visualizzare un segnale elettrico nel tempo.  
Sullo schermo si possono notare le cosiddette **divisioni** (i quadrati) e **sottodivisioni** (le tacche sugli assi $x,y$).  
L'unita delle divisioni puo' essere configurata, mentre le sottodivisioni sono sempre $\frac{1}{5}$ delle divisioni.  
Se per esempio una divisione e' $1V$ allora una sottodivisione sara' $0.2V$.



# Tipi di contatto con un conduttore  

### Contatto diretto  
Si chiama contatto diretto, quando si tocca un cavo, un conduttore direttamente con mano, o comunque con il corpo.  

### Contatto indiretto  
Si chiama contatto indiretto, il contatto che avviene con un dispositivo che per qualche ragione e' a contatto con il cavo e.g. a causa di un malfunzionamento, il cavo tocca il telaio della lavatrice che a sua volta viene in contatto con il nostro corpo.  
Se siamo fortunati, e' stata fatta la messa a terra, e siamo salvi. 


# Cavi elettrici  

|tipo|abbreviazione|colori|
|--|--|--|
|Fase|F|nero, marrone, grigio|
|Neutro|N|blu, celeste|
|Protezione|PE|giallo-verde|

**Sezionare** un cavo significa tagliarlo in modo tale da interrompere la corrente al suo interno, che e' il modo in cui agiscono gli interruttori in un quadro elettrico.  


# Sistema trifase e distribuzione  

![three-phase-optimised](https://user-images.githubusercontent.com/7195133/195997060-739e3a6f-50dc-43cc-ad95-1ba4398a600d.gif)![phase_shift](https://user-images.githubusercontent.com/7195133/195997366-984b02f8-a964-406f-8803-0df44a3f509b.jpg)


Come si intuisce dall'animazione le tensioni (e quindi anche le correnti) prodotte sono **sfasate** di $120\degree$ tra di loro.  
Questo sfasamento in una situazione ideale provocherebbe l'annullamento totale delle correnti al nodo finale di confluenza delle tre fasi, rendendo inutile l'uso del neutro.  
Realisticamente pero' il carico non e' distribuito in modo perfetto, e lo sfasamento puo' variare nel tempo, questo ci permette comunque di utilizzare un solo cavo per il neutro, il quale, se il carico e' distribuito in modo uniforme, vede pochissima corrente, o addirittura nulla.  

![tensione_tra_fase_e_fase](https://user-images.githubusercontent.com/7195133/196024846-cbef5057-09d4-405b-9110-ab75e2e7ddc4.jpg)

Le tensioni in Italia sono $230V$ tra fase e neutro, e $400V$ tra fase e fase.  
E' cruciale rendersi conto che questi sono valori efficaci, la tensione tra due fasi in effetti varia nel tempo, ma per semplicita' ci si riferisce sempre al valore efficace.  
Se fase 1 e 2 sono rispettivamente $f_1 = \sin{x}$ e $f_2 = \sin{-\frac{2\pi}{3}+x}$  
Allora la differenza di potenziale tra loro nel tempo viene descritta da $V_t = f_1 - f_2$  
Il rapporto tra i due valori efficaci e' $\frac{400V_{eff}}{230V_{eff}} \simeq \sqrt{3}$  ovvero  $230V_{eff} * \sqrt{3} \simeq 400_V$  

![trifase_distribuzione](https://user-images.githubusercontent.com/7195133/195996852-ce9eb3f5-564f-4551-8572-958aaddaf72b.jpg)  

Grazie al sistema trifase si possono creare configurazioni con tensioni diverse a seconda delle esigenze, sempre assicurandosi che i carichi siano distribuiti sulle fasi in modo uniforme.







