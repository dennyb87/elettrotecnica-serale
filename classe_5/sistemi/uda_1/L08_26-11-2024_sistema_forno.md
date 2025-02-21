# Controllo automatico di temperatura di un forno  

```mermaid
flowchart LR
    START[ ]--"V<sub>i</sub>"-->node(("#45;"))
    node--"V<sub>e</sub>"-->ctrl-->act-->sys
    sys-->out((" "))--"y"-->STOP[ ]
    out-->sensor
    cond--"V<sub>r</sub>"-->node

    subgraph transducer
        sensor-->cond
    end

    style START width:0px,height:0px;
    style STOP  width:0px,height:0px;
```

1. Un potenziometro fornisce in ingresso una tensione $V_i$ che rappresenta la temperatura desiderata
2. Il blocco di reazione non e' che il trasduttore, questo converte la temperatura rilevata nel forno in una tensione $V_r$
3. il nodo sottrattore produce quindi il segnale di errore $V_e = V_i - V_r$
4. il blocco di controllo e' presente se c'e' bisogno di manipolare il segnale
5. il blocco di attuazione si occupa modificare il sistema in modo proporzionale alla tensione fornita
6. il forno e' il sistema da controllare 


### Principio di funzionamento  

Una volta fissato il valore della tensione di riferimento $V_i$ che rappresenta la temperatura desiderata, al variare della temperatura del forno variera' la tensione del blocco di reazione $V_r$ causando a sua volta una variazione nella tensione di errore $\pm V_e$  

Se la temperatura misurata e' minore di quella desiderata allora si ha un errore positivo che porta all'aumento della quantita di combustibile che a sua volta porta all'aumento della temperatura del forno.  

![sonda_pt_1000_curva_caratteristica](https://user-images.githubusercontent.com/7195133/196776916-a970bb43-232b-44f1-a02b-8b3ab2f3d15d.jpg)  

Per semplicita' impotizziamo l'uso di una sonda *PT1000* che ha resistenza $R_T = 1758.6\ \Omega$ ad una temperatura di $200^\circ C$. La tensione in ingresso $V_i$ che rappresenta la temperatura desiderata sara' allora:  

$V_i = E \cdot \dfrac{R_T}{R_T+R_0} = 12\cdot\dfrac{1758.6}{1758.6+1000} \simeq 7.65\ V$  

Se la temperatura misurata dal sensore e' $200^\circ C$ allora $V_r = V_i = 7.65\ V$ per cui...  

$V_i - V_r = V_e = 0\ V$  

Se invece la temperatura del forno scende $T_r\downarrow$ la tensione in uscita dal blocco di reazione $V_r\downarrow$ scende a sua volta portando ad un segnale di errore positivo che attraverso il blocco di controllo e attuazione aumentera' la temperatura del forno, compensando alla diminuzione di temperatura.  

$V_i = 7.65 \implies \sim 200^\circ C$  
$V_r = 7.12 \implies \sim 120^\circ C$  

$V_i - V_r = V_e = 7.65 - 7.12 = 0.53\ V$  


### Trasduttore  

```mermaid
flowchart LR
    START[ ]--"temperature"-->sensor
    cond--"voltage"-->STOP[ ]
    subgraph transducer
        sensor-->cond
    end

    style START width:0px,height:0px;
    style STOP  width:0px,height:0px;
```

Il trasduttore è un dispositivo di qualsiasi genere destinato a convertire una grandezza fisica in un'altra, effettuando quindi una sorta di *traduzione*. In elettrotecnica si converte quindi una grandezza fisica in una grandezza elettrica, generalmente tensione o corrente. Questo e' composto da un sensore ed un circuito di condizionamento.  

Il **sensore** è un dispositivo in grado di rilevare le variazioni di una grandezza fisica, in questo caso variazioni della temperatura (e.g. sonda *PT1000*). Il sensore risponde con una variazione di resistenza che pero' risulta una grandezza scomoda da utilizzare per governare i circuiti, per cui si sfrutta un **circuito di condizionamento** che converta la resistenza in una tensione.  

![pt1000_transducer](https://github.com/user-attachments/assets/24d53f32-f206-49b4-9fa2-b3533ffd0119)  

In figura vediamo la sonda *PT1000* $R_T$ nel inserita nel circuito di condizionamento alimentato a $12\ V$ la cui uscita e' proprio $V_{R_T}$  
