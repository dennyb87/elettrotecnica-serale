# Diagrammi di Bode  

Un diagramma di Bode permette di rappresentare graficamente la risposta in frequenza di un sistema. Data una funzione di trasferimento $G(s)$ e' possibile trovare la risposta in frequenza con valutando $G(j\omega)$ dove $j\omega$ e' un numero complesso che rappresenta la velocita' angolare del vettore equivalente del segnale in ingresso al sistema.  

![circuit_CR](https://github.com/user-attachments/assets/f2f1213c-5c1f-4450-b941-728656ba6bcd)  

Dato il circuito dove:

$R = 100\ k\Omega$  
$C = 0.1\ mF$  
$RC = 100\cdot 10^3 \cdot 0.1 \cdot 10^-3 = 100 \cdot 0.1 = 10\ s$  

Troviamo la funzione di trasferimento...  

$G(s) = \dfrac{V_{out}}{V_{in}} = \dfrac{R}{\frac{1}{Cs}+R} = \dfrac{RCs}{1+RCs} = \dfrac{10s}{1+10s}$  

Sostituiamo quindi $j\omega$ per trovare il vettore della risposta in frequenza...  

$G(j\omega) = \dfrac{10j\omega}{1+10j\omega}$  

Nel diagramma di Bode viene utilizzato pero' il modulo di $G(j\omega)$ ovvero $|G(j\omega)|$. Essendo interessati al modulo la parte immaginaria puo' essere ignorata, per cui per il teorema di Pitagora al denominatore...  

$|G(j\omega)| = \dfrac{10\omega}{\sqrt{1 +100\omega^2}}$  

Valutiamo ora i limiti per $\omega \to +\infty$ e $\omega \to 0^+$...  

$\displaystyle{\lim_{x\to +\infty}}\ |G(j\omega)| = \dfrac{10\omega}{\sqrt{\omega^2\bigg(\dfrac{1}{\omega^2}+100\bigg)}} = \dfrac{10\cancel{\omega}}{\cancel{\omega}\sqrt{0+100}} = 1$  

$\displaystyle{\lim_{x\to 0^+}}\ |G(j\omega)| = \dfrac{10\omega}{\sqrt{\omega^2\bigg(\dfrac{1}{\omega^2}+100\bigg)}} = \dfrac{10\cancel{\omega}}{\cancel{\omega}\sqrt{+\infty+100}} = 0$  

Scopriamo quindi che la il circuito e' un filtro passa alto, in quanto ad alte frequenze in ingresso il sistema fa passare tutto il segnale, mentre a frequenze basse viene non si ha alcun segnale in uscita. Di seguito il **diagramma di Bode** del sistema, ovvero il grafico della sua risposta in frequenza.  

![filtro_passa_alto](https://github.com/user-attachments/assets/d01e7852-a120-4a42-82b1-bf86de9b92e3)  

Per definizione la frequenza di taglio $\omega_t$ e' l'inverso della costante di tempo $\tau$ ovvero:  

$\omega_t = \dfrac{1}{\tau}$  

In questo caso...  

$\omega_t = \dfrac{1}{\tau} = \dfrac{1}{RC} = \dfrac{1}{10} = 0.1\ \frac{rad}{s}$  

Valutando $|G(\omega_t)|$ troviamo allora che...  

$|G(\omega_t)| = \dfrac{10\cancel{\omega_t}}{\cancel{\omega_t}\sqrt{\bigg(\dfrac{1}{\omega_t^2}+100\bigg)}} = \dfrac{10}{\sqrt{(100+100)}} = \dfrac{10}{\sqrt{100(1 + 1)}} = \dfrac{\cancel{10}}{\cancel{10}\sqrt{2}} = \dfrac{1}{\sqrt{2}} = \dfrac{\sqrt{2}}{2}$  

L'ordinata $\dfrac{\sqrt{2}}{2}$ rappresenta quindi il punto di discriminazione della funzione di trasferimento.  

## Risposte in frequenza dei filtri piu' comuni  

E' possible costruire diversi tipi di filtri tra cui:  

* filtro passa-basso
* filtrp passa-altro
* filtro passa-banda
* filtro elimina-banda

![common_filters](https://github.com/user-attachments/assets/f306bee6-7670-4b8e-991e-2df6fc7a725f)  
