# Sensore termico  

Il sensore è un dispositivo in grado di rilevare le variazioni di una grandezza fisica, in questo caso variazioni della temperatura.  
Prendiamo in considerazione la sonda **PT 1000**.  

![sonda_pt1000](https://user-images.githubusercontent.com/7195133/196768275-185179a4-7439-4edd-8dee-8c97744dc6db.jpg)

**PT** sta per Platino, mentre **1000** indica una resistenza di $1k\Omega$ alla temperatura di $0\degree$  
Il punto chiave, ed e' un dettaglio importante di cui non eravamo ancora a conoscenza, e' che **la resistenza di  
un componente varia al variare della temperatura**. 


Il motivo fisico e' che il reticolo cristallino del materiale, in questo caso il platino, si eccita sempre di piu' all'aumentare della temperatura.  
Gli elettroni quindi fanno piu' fatica a passare, trovano quindi piu' resistenza, un po' come cercare di arrivare da un punto $A$ and un punto $B$ passando attraverso una folla in movimento.  

![cold_wire](https://user-images.githubusercontent.com/7195133/196873501-7b4e8d49-ea2c-4efd-b147-193afbe032a0.gif)![warm_wire](https://user-images.githubusercontent.com/7195133/196873710-939b2e0a-3e3d-41a5-9b11-3443be1f51d9.gif)


Tra resistenza e temperatura esiste una **relazione lineare** per cui al variare di un grado  
si ha sempre la stessa variazione di resistenza.  

![sonda_pt_1000_curva_caratteristica](https://user-images.githubusercontent.com/7195133/196776916-a970bb43-232b-44f1-a02b-8b3ab2f3d15d.jpg)


Cio' significa che fornendo una corrente (o una tensione) al sensore si potra' misurare una variazione di tensione (o corrente)  
al variare della temperatura, e se la corrente (o tensione) e' nota di consequenza derivare la temperatura.   
Se forniamo per esempio $1A$ a $0\degree$ si avrebbe $1A \cdot 1000\Omega = 1000V$ mentre a $1\degree$ si avrebbe $1A \cdot 1003.9\Omega = 1003.9V$.  

![sensore_termico](https://user-images.githubusercontent.com/7195133/196773124-78c8359f-7d12-4655-841e-e13ae34b2bbd.jpg)

Dato che la relazione e' lineare si puo' sempre derivare uno dei due valori, resistenza o temperatura, conoscendo la pendenza della retta  
ovvero $\frac{\Delta{\Omega}}{\Delta{\degree{C}}}$ per quella particolare sonda o materiale, nel caso della sonda PT 1000  
si hanno $3.9\Omega$ di variazione per grado centigrado.  

Se non si vogliono fare calcoli si possono comunque trovare le tabelle di conversione.  

![tabella_conversione_pt_1000](https://user-images.githubusercontent.com/7195133/196774573-06780e7c-c8db-4934-b7d8-10b7caa87dcf.jpg)  

Per trovare la resistenza del sensore a $25\degree$ basta andare nella casella di riga $20$ colonna $5$.  
A $25\degree$ la sonda PT 1000 ha quindi una resistenza di $1097.3\Omega$


