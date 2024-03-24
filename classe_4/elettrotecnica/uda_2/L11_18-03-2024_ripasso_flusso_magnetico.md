# Produzione di flusso magnetico  

Esistono tre metodi principali per produrre flusso magnetico:

1. movimento relativo
2. autoinduzione
3. mutua induzione

## Flusso per movimento relativo  

![relative_motion](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/fe206b25-197d-4405-8875-5c23979bcc83)  

Il movimento del magnete rispetto al solenoide, o viceversa, induce una tensione sul solenoide e di conseguenta corrente.  

## Autoinduzione  

![autoinduzione](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/fbc28fbc-7996-40f7-95d0-7d8fb7c8afdd)  

Nel momento in cui la corrente attraversa un conduttore si produce flusso magnetico, in questo caso dato il solenoide si ha un flusso concatenato. E' importante notare che l'autoinduzione si manifesta per implicazione anche nel primo metodo per movimento relativo.  

## Mutua induzione  

![mutual_induction](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c1b947ba-33f3-4c74-9ff1-cbfe8348f20c)  

Alimentando un circuito primario $P$ e' possibile alimentare un circuito secondario $S$. In particolare il flusso autoindotto del primario attraversa il secondario inducendovi una tensione e quindi una corrente.  

# Legge di Hopkins  

La legge di Hopkins ci e' l'equivalente di Ohm nel circuito magnetico e mette in relazione la forza magnetomotrice $I$ con il flusso $\phi$ ed una quantita' che rappresenta l'opposizione al flusso, la riluttanza $\mathcal{R}$  

$N \cdot I = \mathcal{R} \cdot \phi$  

Dove $N$ e' il numero di spire mentre $\mathcal{R} = \dfrac{\ell}{S\mu}$ in cui $\ell$ e' la lunghezza del solenoide $S$ la sua sezione, e $\mu$ la permeabilita' magnetica del materiale. Sapendo che in un solenoide il flusso concatenato e' $\phi_c = N \cdot \phi$ si puo' concludere che...  

$\phi_c = N \cdot \phi = N \cdot \dfrac{N \cdot I}{\mathcal{R}} = \dfrac{N^2}{\mathcal{R}} \cdot I = L \cdot I$  

Si ha allora che $L = \dfrac{N^2}{\mathcal{R}}$ prende il nome di **induttanza** e dipende dalla geometria e dal materiale del componente. Questa rappresenta sia la bonta' con cui il componente riesce a produrre flusso, e per via della conseguente autoinduzione, anche anche l'attitudine del componente ad opporsi alla variazione di corrente.  
