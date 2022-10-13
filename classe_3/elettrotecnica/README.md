> 15/09/2022

# Effetti della corrente

 |Effetto|Descrizione|
 |---|---|
 |termico|Gli atomi del conduttore vengono urtati dagli elettroni in movimento riscaldandosi.|
 |luminoso|Quando gli elettroni eccitati passano ad uno stato di minore energia vengono emessi quanti di luce (fotoni).|
 |magnetico|Le cariche in movimento generano un campo magnetico|
 |chimico|Negli elettroliti gli ioni si spostano verso gli elettrodi. Questo processo può separare gli ioni di carica opposta sciogliendone i legami.|
 |piezoelettrico|Alcuni cristalli reagiscono al cambiamento di tensione con una deformazione meccanica.|
 |elettrostatico|Elettrizzazione per strofinio di materiali isolanti, laforza d'attrito agisce in modo tale da "strappare" elettroni da uno dei due materiali|
 |fisiologico|La corrente puo avere effetti sul corpo umano con conseguenze anche mortali|
 
 
# Strumenti di misura

### Amperometro

Misura la corrente sche scorre in un conduttore in **Ampere** con simbolo **A** e si collega in serie.  
In un analogia idraulica, per misurare quanta acqua passa in un tubo, si deve intervenire sul tubo, inserendo una sorta di contatore. 

```mermaid
graph LR
    START[ ]---A((A))
    ---STOP[ ]
    style START fill:#FFFFFF, stroke:#FFFFFF;
    style STOP  fill:#FFFFFF, stroke:#FFFFFF;
```

### Voltmetro

Misura la tensione tra due punti in **Volt** con simbolo **V** e si collega in parallelo.
Puo misurare una tensione negativa e.g. -9V in questo caso significa che ho invertito i puntali, in quanto il segno indica la polarita del circuito. 

```mermaid
graph LR
    START[ ]---A((V))
    ---STOP[ ]
    style START fill:#FFFFFF, stroke:#FFFFFF;
    style STOP  fill:#FFFFFF, stroke:#FFFFFF;
```

### Ohmmetro

Misura la resistenza di uno o piu resistori in **Ohm** con simbolo **Ω**

```mermaid
graph LR
    START[ ]---A((Ω))
    ---STOP[ ]
    style START fill:#FFFFFF, stroke:#FFFFFF;
    style STOP  fill:#FFFFFF, stroke:#FFFFFF;
```

# Legge di Ohm

$V = IR$  
$\frac{V}{I} = R$  
$\frac{V}{R} = I$  

Una tensione **V** su una resistenza **R** produce una corrente **I**.  
La tensione e' la causa della corrente elettrica.  


 |R[Ω]|V[V]|I[A]|P[W]|
 |---|---|---|---|
 |10|0|0|0|
 |10|5|0.5|2.5|
 |10|10|1|10|
 |10|15|1.5|22.5|
 |10|20|2|40|

### Potenza

$P = VI$  
$P = \frac{EN}{t}$  

La potenza equivale all'energia fornita o assorbita (o lavoro compiuto) nell'unita di tempo, si misura in **Watt** con simbolo **W**.  
In un certo senso e' la velocita con cui il lavoro viene compiuto dato che $P = \frac{W}{t}$.


# Multimetro

![multimetro_simboli](https://user-images.githubusercontent.com/7195133/195452312-d78da9f5-85aa-4c4d-a259-316bc03646a6.png)

### Portata

La portata e' il valore massimo che lo strumento puo misurare, e' configurabile entro i limiti della portata massima.  
Nel dubbio, seleziona la portata maggiore e poi scendi per non danneggiare lo strumento.  
Ci sono **strumenti analogici**, riconoscibili da una **scala graduata** e.g. una bilancia, e **strumenti digitali** dove la misura viene indicata direttamente con dei **numeri su un display** e.g. orologio digitale.

### Misure e notazione scientifica

 |Base 10|Nome|Simbolo|Decimale|
 |--|--|--|--|
 |$10^6$|mega|M|1000000|  
 |$10^3$|kilo|k|1000|  
 |$10^2$|hecto|h|100|  
 |$10^1$|deca|da|10|  
 |$10^0$|_|_|1|  
 |$10^-1$|deci|d|0.1|
 |$10^-2$|centi|c|0.01|
 |$10^-3$|milli|m|0.001|
 |$10^-6$|micro|μ|0.0001|
