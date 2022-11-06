# Grandezze fisiche, dimensioni, e unita' di misura

Una grandezza fisica e' la caratteristica di un oggetto misurabile e.g. la lunghezza di un tavolo.  
Ci sono grandezze fondamentali e derivate, queste si esprimono con una dimensione che puo' essere costituita da una o piu' grandezze fondamentali.  
Ad esempio la dimensione della lunghezza che ' una grandezza fondamentale e' $L$ (lunghezza ovviamente), mentre la dimensione dell'area che e' invece derivata e' $L^2$.

```mermaid
graph TB
    A(Grandezze fisiche)
    B(Area)
    C(Dimensione)
    D(Unita' di misura)
    E("L#178;")
    F("m#178; ft#178; ...")
    A --> B
    B --> C & D
    C --> E
    D --> F
```  

Come si nota in figura le grandezze hanno una ed una sola dimensione, ma possono avere piu' unita' di misura. 

Si puo' usare la notazione $[...]$ per estrarre l'unita' di misura da una dimesione e.g. $[L] = m$  
Questo equivale a dire che l'unita' di misura della lunghezza e' il *metro*.  
Oppure $[I] = A$ ovvero l'unita' di misura della corrente e' l'*Ampere*.  

# Schemi di montaggio

![schema_di_montaggio](https://user-images.githubusercontent.com/7195133/200169419-25479ceb-4a30-4929-b3e5-730c5deabdf6.jpg)  

Lo **schema di montaggio** e' uno schema in scala che mostra le connessioni tra i diversi elementi dell'impianto, rispettando le loro posizioni.  

# Circuiti elettrici equivalenti

![circuito_elettrico_equivalente](https://user-images.githubusercontent.com/7195133/200169389-38e37b79-fef2-49db-a460-b70fbf638bb5.jpg)  

Il **circuito elettrico equivalente** e' invece una rappresentazione semplificata del circuito reale.  
Semplificata perche' non deve essere in scala ne' rispettare le posizioni dei componenti.  

Nel circuito elettrico si devono indicare i punti di collegamento specificando se sono **punti semplici** o **nodi**, le grandezze elettriche fondamentali, e la direzione della corrente convenzionale.  

I **punti semplici** sono punti che collegano due elementi di filo conduttore.  
Sono invece **nodi** se collegano almeno tre elementi di filo conduttore.  

![punti_semplici_e_nodi](https://user-images.githubusercontent.com/7195133/200171084-0d9c5873-81e7-48eb-b5b3-5648f2da4cb2.jpg)  

Nella figura, $F$ e $B$ sono nodi, tutti gli altri invece sono punti semplici.  


# Pila ideale e pila reale  

![pila_ideale_e_reale](https://user-images.githubusercontent.com/7195133/200162627-463aa5d4-3ac2-4490-aced-19e8c0946431.jpg)  

Un componente come un conduttore o una pila, puo' essere rappresentato ignorando dettagli trascurabili come la resistenza interna, in questo si dice che e' **ideale**.  
Si dice invece **reale** quando si tiene conto di questi dettagli, che rendono il modello molto piu' accurato. La descrizione del componente diventa quindi molto vicina alla realta'.  

![curva_caratteristica_pila_reale](https://user-images.githubusercontent.com/7195133/200162981-7523217c-7523-4ae4-b9f7-9c3f90d945fa.jpg) 

Se vogliamo che la nostra descrizione del comportamento di una pila sia piu' vicino alla realta' dobbiamo allora tenere conto della sua resistenza interna (vedi $R_s$ in figura).  
Si intuisce quindi che se la pila ha una resistenza interna, allora ci deve essere una caduta di potenziale su quest'ultima.  
Ne consegue che la tensione effettiva in uscita dalla pila $V_{out}$ sara' sempre minore di $V_s$ in dipendenza di $R_s$.  

