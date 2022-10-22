# Reattanza 

In corrente alternata, quando si ha un carico puramente resistivo, corrente e tensione sono **in fase**.  
Essere in fase significa che i picchi sono sincronizzati nel tempo, i segnali raggiungono quindi 
i rispettivi valori massimi, che possono essere diversi, nello stesso momento, come in figura.  

![corrente_e_tesione_in_fase](https://user-images.githubusercontent.com/7195133/196049529-274c8e90-671a-4ebb-8d06-e707c4a05f32.jpg)

Quando invece si ha un carico con una **componente reattiva** (induttiva o capacitiva), allora si otterra'  
un effetto di sfasamento causato dalla natura stessa dei componenti.  

![corrente_e_tensione_sfasate](https://user-images.githubusercontent.com/7195133/196050137-2c2223d8-5c31-4c85-9cbf-179975b1b80e.jpg)

Questi componenti si comportano in un certo senso come dei resistori, in quanto a seconda della frequenza   
presentano una certa opposizione al passaggio della corrente, immagazzinando energia ma senza dissiparla  
(si veda il funzionamento di induttori e capacitori) e che quindi viene restituita al circuito.   
Bisogna ricordare che pur non essendoci consumo (in realta' c'e' ma trascurabile perche' molto piccolo)  
questa energia deve essere comunque fornita per far funzionare i componenti.  

![reactance_phase_shift](https://user-images.githubusercontent.com/7195133/196050549-4a9faf75-78cb-4097-b396-39d5618ad823.jpg)


# Reattanza capacitiva 

Un carico puramente capacitivo causa uno sfasamento dove la corrente e' in anticipo di $90\degree$ rispetto alla tensione.


# Reattanza induttiva  

Un carico puramente induttivo causa uno sfasamento dove la corrente e' in ritardo di $90\degree$ rispetto alla tensione.


# Impedenza

Quando il carico non e' puramente resistivo, e ci sono quindi componenti reattive, si parla allora di **impedenza**  
ovvero un impedimento al passaggio di corrente, che e' piu complesso di una semplice resistenza.  

L'impedenza si indica con $Z$ e si misura in Ohm in quanto presenta un'opposizione al passaggio di corrente come una resitenza.   
La derivazione della formula verra' affrontata piu avanti, per adesso e' sufficiente sapere che a causa dei diversi comportamenti  
di reattanze e resistenze, non e' possibile semplicemente sommarle tra loro ma viene calcolato il modulo di una somma vettoriale  
dove i due vettori rappresentano rispettivamente la resistenza $\vec{R}$ e la reattanza $\vec{X}$.  

$|\vec{Z}| = \sqrt{\vec{R}^2 + \vec{X}^2}$  


# Fattore di potenza  

Abbiamo capito che in corrente alternata in un circuito con componenti reattive si puo' avere uno sfasamento tra corrente e tensione.  
Questo sfasamento si puo' rappresentare con un angolo generalmente chiamato $\varphi$ (Phi pronunciato *"fi"*).  

Ad esempio, la potenza assorbita da un circuito senza componenti reattive in cui scorre $1A$ con un generatore da $1V$ e' di un $1W$  
In questo caso l'angolo di sfasamento e' zero, per cui la formula della potenza equivale a $P = V \cdot I \cdot \cos{\varphi}$  
Visto che l'angolo e' zero, allora $\cos{\varphi} = 1$ e di consequenza vale la legge di Ohm $P = V \cdot I$  

Nel caso in cui si abbiano componenti reattive, l'angolo di sfasamento diventa maggiore di zero, si presenta quindi quello che chiamiamo  
un **fattore di potenza**, il quale ci che ci permette di fare una distinzione tra potenza **apparente** $S$, **attiva** $P$, e **reattiva** $Q$.  

$P = V \cdot I \cdot \cos{\varphi}$  
$Q = V \cdot I \cdot \sin{\varphi}$  
$S = V \cdot I$  

Come si intuisce dalle equazioni, la potenza apparente non e' altro che la somma tra potenza attiva e reattiva $S = P + Q$  
La potenza apparente si misura in **VA** *Volt-Ampere*, la reattiva in **VAR** *Volt-Ampere Reattivi*, mentre l'attiva in **W** *Watt*. 


![cos_phi](https://user-images.githubusercontent.com/7195133/197002051-9a1842fe-8312-4a1b-b046-81e82736785e.jpg)

In figura viene ripetuto quanto detto ma in uno spazio vettoriale dove $|S| = \sqrt{\vec{P}^2+\vec{Q}^2}$

La potenza attiva e' la potenza effettivamente assorbita dai carichi resistivi, mentre la potenza reattiva e' quella potenza che  
pur non essendo effettivamente dissipata deve essere fornita per il funzionamento del circuito.   
Il fornitore di energia non e' contenta di dover fornire $Q$ perche significa che comunque in qualche modo deve generarla con i relativi costi.  
Quindi il fornitore (L'Enel per esempio) mette una soglia di $0.95$ per cui se un impianto ha un $\cos{\varphi}$ inferiore dovra' pagare una penale.  
Si consiglia in genere di rifasare l'impianto in questi casi, quindi apportare le appropriate modifiche, aggiungendo i componenti necessari (capacitori o induttori) capaci di riportare la corrente in fase con la tensione.   
Realisticamente pero un $\cos{\varphi} = 1$ e' impossibile da raggiungere in quanto anche un semplice cavo puo' assumere i comportamenti di un induttore o di un capacitore.  




