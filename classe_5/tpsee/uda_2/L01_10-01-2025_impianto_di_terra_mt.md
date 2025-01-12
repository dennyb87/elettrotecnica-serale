# Impianti di terra in media tensione (MT)  

L'impianto MT dell'ente distribuzione puo' avere neutro isolato o compensato. Isolato significa appunto isolato da terra, mentre il neutro compensato prevede l'installazione di una componente induttiva detta *bobina Petersen*.  

![simple_petersen_coil](https://github.com/user-attachments/assets/0c596afc-1124-4143-9071-a4140b97ba51)  

In caso di guasto la corrente scaricherebbe a terra, questo essendo un conduttore, crea una componente capacitiva con le fasi dell'impianto, facendo richiudere il circuito causando delle correnti molto grandi. La bobina serve allora in un certo senso a *"rifasase"* il circuito, diminuendo cosi' la corrente, e di conseguenza aumentando i tempi di intervento permettendo cosi' di installare interruttori selettivi.  

L'ente distribuzione ci comunica le correnti di guasto e i tempi di intervento in dipendenza del tipo di neutro.

* **neutro isolato**
  * $200/300\ A$
* **neutro compoensato**
  * $50\ A - 20\ kV$
  * $40\ A - 15\ kV$

![tempi_intervento_mt](https://github.com/user-attachments/assets/2c5f663d-b9c7-4ea6-af20-57b374d98118)  

La tensione di contatto limite $U_{tp}$ varia al variare del tempo di permanenza della corrente di guasto. Con tempi minori si ha una probabilita' di contatto minore e quindi sono ammesse tensioni di contatto limite maggiori.  

## Esempio di installazione  

Ipotizzando un impianto a neutro compensato con $40\ A - 15\ kV$ ed un tempo di intervento $\gt\gt 10\ s$ si hanno quindi:  

$I_F = 40\ A$  
$U_{tp} = 80\ V$  

Dove $I_F$ e' la corrente di terra che viene utilizzata a fini cautelativi in quanto questa, rappresenta in realta' solo circa il 70% della corrente di guasto totale (il restante 30% si richiude sulla schermatura dei cavi). Si vuole allora soddisfare la relazione:  

$R_E \le \dfrac{U_{tp}}{I_F}$  

Nel nostro caso $\dfrac{U_{tp}}{I_F} = \dfrac{80}{40} = 2\ \Omega$ per cui...  

$R_E \le 2\ \Omega$  

In media tensione si evita l'utilizzo dei picchetti in quanto si vuole ottenere una superficie piu' equipotenziale possibile, per cui si preferisce ad esempio l'installazione di una rete magliata che sfrutta i dispersori di fatto come plinti di fondazione e/o reti elettrosaldate.  

### Calcolo resistenza di terra  

![rete_magliata](https://github.com/user-attachments/assets/ce2620f6-c020-4345-8c59-7e0934c4c0ef)  

Ipotizzando un capannone $10\ m \times50\ m$ si vuole installare quindi una rete magliata in corda di rame nudo di $25\ mm^2$ considerando una resistivita' del terreno di $300\ \Omega m$. La formula per impianti di terra realizzati con reti magliate e' la seguente:  

$R_E = \dfrac{\rho_\epsilon}{4r}+\dfrac{\rho_\epsilon}{L}$  

Dove $r$ e' il raggio di un cerchio di area equivalente della rete, mentre $L$ rappresenta tutta la lunghezza del dispersore.  

Troviamo quindi l'area del cerchio equivalente...  

$A = 10\cdot50 = 500\ m^2$  

$A = \pi r^2 \implies r = \sqrt{\dfrac{A}{\pi}} = \sqrt{\dfrac{500}{\pi}} \simeq 12.62\ m$  

Per calcolare invece tutta la lunghezza del dispersore occorre invece contare i tratti di dispersore verticali $5$ e quelli orizzontali $3$ e moltiplicarli per le relative lunghezze...   

$L = 3\cdot 50 + 5\cdot 10 = 200\ m$  

$R_E = \dfrac{\rho_\epsilon}{4r}+\dfrac{\rho_\epsilon}{L} = \dfrac{300}{4\cdot 12.62} + \dfrac{300}{200} \simeq 7.44\ \Omega$  

L'impianto di terra non soddisfa quindi la condizione $R_E \le 2\ \Omega$, dovremmo allora procedere ad aumentare l'area della rete magliata, rivedere la resistivita' del terreno etc.. o potenzialmente considerare la condizione soddisfatta grazie all'utilizzo dei dispersori di fatto.  
