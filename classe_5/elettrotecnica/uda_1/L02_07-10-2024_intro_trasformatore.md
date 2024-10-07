# Introduzione al trasformatore elettrico  

![simple_transformer](https://github.com/user-attachments/assets/5791700b-60aa-491d-8936-9727f8c1f120)  

Il trasformatore e' una **macchina elettrica** che appunto trasforma l'energia elettrica cambiandone i parametri di tensione e corrente. E' composto da un nucleo ferromagnetico su cui vi sono un avvolgimento primario ed uno secondario. Si dice macchina elettrica un dispositivo in grado di trasformare energia sfruttando le leggi dell'elettromagnetismo, in particolare:  

* legge di *Faraday-Neumann-Lenz*
* legge di *azione elttrodinamica*

La prima ci dice che la variazione di flusso magnetico nel tempo produce una tensione indotta. La seconda ci dice che un conduttore percorso da corrente immerso in un campo magnetico e' soggetto ad una forza.  

## Rendimento  

```mermaid
graph LR
    p1(("P<sub>1</sub>"))-->ME
    ME-->p2(("P<sub>2</sub>"))
    ME-->P(("P<sub>P</sub>"))
```

$\eta = \dfrac{P_2}{P_1}$  

Il trasformatore, come ogni macchina elettrica, ha un rendimento $\eta$ definito come il rapporto tra potenza in uscita e quella in entrata. Rispetto alle macchina rotanti e.g. un motore, il trasformatore, essendo una **macchina statica**, ha un rendimento maggiore in quanto non ci sono perdite per *effetto Joule* dovute al movimento di parti meccaniche.  

E' importante notare che il sistema ha sempre delle perdite $P_P$ per cui possiamo riscrivere l'equazione come...  

$\eta = \dfrac{P_2}{P_1} = \dfrac{P_1-P_P}{P_1} = 1 - \dfrac{P_P}{P_1}$  

Il trasformatore e' soggetto a due perdite principali:  

* perdite per *effetto Joule* $P_j$
* perdite per *perdite del ferro* $P_f$

## Perdite Joule  

$P_j = RI^2$  

La perdita per effetto Joule e' dovuta al tipo di materiale dei conduttori con cui viene realizzato il trasformatore e.g. rame, alluminio. Questa dipende quindi dalla resistenza $R$ del materiale.  

## Perdite del ferro  

$P_f = Pi + P_{cp}$  

Le perdite del ferro $P_f$ hanno a che fare con il nucleo magnetico, e hanno due componenti:
* perdite per *isteresi* $P_i$
* perdite per *correnti parassite* $P_{cp}$

Le perdite per isteresi si hanno in quanto parte dell'ernergia deve essere spesa per orientare i domini magnetici in direzione del flusso.  

$P_i = K_i \cdot f \cdot B_M^n$  

Dove $K_i$ tiene conto del materiale del nucleo, $f$ e' la frequenza, mentre $B_M$ e' l'induzione massima.  
