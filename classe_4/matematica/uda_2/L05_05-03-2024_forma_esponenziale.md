# Complessi in forma esponenziale  

Per farci un'idea della la forma esponenziale dobbiamo prima introdurre il **numero di Eulero**. Questa costante fu scoperta affrontando il problema dell'interesse composto, ovvero il calcolo del montante $M$ dato un capitale iniziale $C$ sul quale viene calcolato un interesse $r$ ad $n$ intervalli per $t$ anni (o $t$ volte).  

$M(t) = C\bigg(1 + \dfrac{r}{n}\bigg)^{nt}$  

Se avvessimo ad esempio:  

* capitale iniziale $€\ 100$ quindi $C = 100$
* un interesse del $100$ % ovvero $r = 1$
* maturazione di una volta l'anno $n = 1$
* con 3 anni di investimento $t = 3$

$M(5) = 100\bigg(1 + \dfrac{1}{1}\bigg)^{1 \cdot 3} = 10\cdot 2^3 = €\ 800$  

![compound_interest](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/21dd6f6a-5687-4e51-8e44-ceea7a5436bc)  

Vengono maturati $€\ 100$ nel primo anno, $€\ 200$ nel secondo e $€\ 400$ nel terzo, per un totale di $€\ 700$ di interesse che sommati al capitale iniziale danno un montante di $€\ 800$.  

## Formula di Eulero  

Di seguito una delle definizioni del numero di Eulero:  

$e^x = \underset{n \to \infty}{\lim} \bigg(1+\dfrac{x}{n}\bigg)^n$  

In particolare la costante irrazionale si ricava valutanto il limite con $x = 1$ ed $n$ che tende a infinito:  

$e = \underset{n \to \infty}{\lim} \bigg(1+\dfrac{1}{n}\bigg)^n \simeq 2.718$  

Dopo aver in qualche modo definito $e$ assumiamo che $\dfrac{x}{n} = \theta$ sia un angolo molto piccolo quando $n$ diventa molto grande, per cui dal teorema di De Moivre...  

$(\cos \theta + i\sin \theta)^n = \cos n\theta + i\sin n\theta$  

Si ha che:  

$\bigg(\cos \dfrac{x}{n} + i\sin \dfrac{x}{n}\bigg)^n = \cos x + i\sin x$  

Il primo membro al contrario del secondo, dipende da $n$ e se l'equazione e' vera per ogni $n$ allora e' vera anche nel limite...  

$\underset{n \to \infty}{\lim}\bigg(\cos \dfrac{x}{n} + i\sin \dfrac{x}{n}\bigg)^n = \cos x + i\sin x$  

Dall'approssimazione per angoli piccoli si ha che:  

$\cos \theta \simeq 1$  
$\sin \theta \simeq \theta$  

allora...  

$\underset{n \to \infty}{\lim}\bigg(1 + \dfrac{ix}{n}\bigg)^n = \cos x + i\sin x$  

$\cos x + i\sin x = e^{ix}$  

## Identita' di Eulero  

Dopo aver in qualche modo derivato la formula di Eulero generale vogliamo esaminare il caso particolare dove $x = \pi$  

$e^{i\pi} = \cos \pi + i\sin \pi = -1$  

Riarrangiando troviamo che...  

$e^{i\pi} +1 = 0$  

Considerata una delle formule piu' straordinarie in quanto contiene:  

* l'elemento neutro dell'addizione $0$
* l'elemento neutro della moltiplicazione $1$
* $\pi$ elemento fondamentale della trigonometria
* $e$ altra costante fondamentale
* l'unita' immaginaria $i$

## Operazioni in forma esponenziale  

Sapendo che $\cos x + i\sin x = e^{ix}$ possiamo allora descrivere numeri complessi in forma esponenziale utilizzando le proprieta' delle potenze.  

$3e^{i\pi} \cdot 2e^{i\pi} = 6e^{i(\pi+\pi)} = 6e^{i2\pi} = 6e^{(i\pi)^2} = 6 \cdot (-1)^2 = 6$  
