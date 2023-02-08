# Magnetismo  

Esiste in natura un minerale di ferro chiamato *magnetite* che ha la proprieta' di attirare il ferro, si definisce quindi un *magnete naturale*. Se strofiniamo pezzi di acciaio contro la magnetite anche questi acquisteranno tale proprieta' e si definiscono quindi *magneti artificiali*. Immegergendo un magnete nella limatura di ferro si puo' osservare che questo si concentra maggiormente agli estremi del magnete, questi estremi sono detti poli, per convenzione **polo nord** e **polo sud**.  

Sperimentando con due magneti si puo' osservare che poli diversi si attraggono mentre i poli si respingono. Vediamo un esempio in figura dove si mostrano le linee di campo, che per convenzione vanno da nord a sud.  

![magnetic_field_lines](https://user-images.githubusercontent.com/7195133/216831059-cad37b16-0b5f-4328-91b4-58f6f11f24c3.jpg)

L'esperienza ci mostra anche che non e' possibile isolare i poli di un magnete, ma che dividendo una calamita si ottengono altre calamite complete piu' piccole.  

![cannot_create_monopoles](https://user-images.githubusercontent.com/7195133/216831364-ebd0fcd3-3e47-4bc0-af12-42d06347ba85.jpg)  


# Legge di Coulomb magnetica  

Coulomb ha studiato quantitativamente le attrazioni e le repulsioni tra due poli magnetici, scoprendo che obbediscono ad una legge del tutto simile a quella delle cariche elettriche, e a quella gravitazionale. Egli indico la *"quantita' di magnetismo"* residente sui poli come **massa magnetica**.  

> Due poli di massa magnetica $m_1$ ed $m_2$ esercitano uno sull'altro una forza $F$ direttamente proporzionale alle loro masse, e inversamente proporzionale al quadrato della loro distanza $d$

$F = k \cdot \dfrac{m_1 \cdot m_2}{d^2}$  

Dove:
* $F$ = forza in newton $[N]$
* $m$ = massa magnetica in weber $[Wb]$ 
* $d$ = distanza in metri $[m]$
* $k$ = coefficiente di proporzionalita' $[N \cdot m^2/Wb^2]$

La costante $k$ dipende dal mezzo in cui le masse sono immerse, nel vuoto (praticamente anche nell'aria) vale $63\,326\ Nm^2/Wb^2$  

# Intensita' di campo magnetico  

La legge di Coulomb ci permette di introdurre il concetto di **campo magnetico**, ovvero lo spazio in cui un magnete eserecita un influenza su altri poli immersi in esso. L'intensita' di campo in un punto $A$ e' definita come la forza esercitata da una **massa magnetica sorgente** $m_s$ sul polo nord di una massa magnetica di prova al punto $A$ che ha per definizione una influenza trascurabile e quindi ignorata.  

![intensita_di_campo](https://user-images.githubusercontent.com/7195133/216842816-8cd6fbb2-4aff-4dc8-a7a9-dbcede592cde.jpg)  

$\vec{F_1} = + k \cdot \dfrac{m_s}{d_1^2} \cdot \hat{r_1}$  

$\vec{F_2} = - k \cdot \dfrac{m_s}{d_2^2} \cdot \hat{r_2}$  

$\vec{H} = \vec{F_1} + \vec{F_2}$  


Dove $F_1$ e' la componente della forza esercitata dal polo nord, ed $F_2$ la componente della forza esercitata dal polo sud, mentre $\hat{r}$ sono i versori nelle rispettive direzioni. Si ha allora che il vettore risultante $\vec{H}$ rapresenta **l'intensita' di campo magnetico** in ampere/metro $A/m$ oppure newton/weber $N/Wb$.  

A questo punto e' importante notare che data una massa magnetica $m$ posta al punto $A$ questa subira' una forza $\vec{F}$ da $m_s$ uguale a $m \cdot \vec{H}$ in newton $N$.  


# Teoria semplificata del magnetismo 

E' sperimentabile che una corrente crea un campo magnetico, allora anche gli elettroni orbitando intorno al nucleo degli atomi in un qualunque materiale rendono ogni atomo un piccolo magnete.  

![atomo_magnete](https://user-images.githubusercontent.com/7195133/217607917-1dcb8752-e810-47e1-ac67-1cec61bb8591.jpg)  

Nella maggior parte dei materiali le orbite sono orientate in modo casuale per cui la somma dei campi magnetici e' pressoche' nulla.  

![random_orbitals](https://user-images.githubusercontent.com/7195133/217608451-212dfeb8-44ab-48be-adac-f3002c8f1491.jpg)  

Talvolta pero' un materiale puo' presentare orbite orientate o naturalmente o per via di un influenza magnetica indotta. Nei casi in cui ci sia un allineamento naturale dei *magnetini elementari* si dice che il materiale e' un **magnete naturale**.

![oriented_orbitals](https://user-images.githubusercontent.com/7195133/217609502-56fa5bfd-b2b5-4d27-b32e-0c45a9361fb0.jpg)  

Quando si immerge un materiale in un campo magnetico possono succedere due cose:

1. l'asse magnetico dei magnetini elementari si orienta in verso opposto a quello del campo applicato, in questo caso si parla di materiale **diamagnetico**
2. l'asse magnetico dei magnetini elementari si orienta nello stesso verso del campo applicato, si parla invece di materiale **paramagnetico**

# Induzione magnetica  

Per **induzione magnetica** si intende quel fenomeno per cui se immergiamo un oggetto di ferro o ferromagnetico in un campo magnetico questo verra' magnetizzato, si dice allora che l'oggetto e' stato magnetizzato per induzione. Osservando lo spettro magnetico con e senza la presenza dell'oggetto, si puo' notare un cambiamento nelle linee di forza. In partcolare il campo diventa piu' intenso in presenza dell'oggetto. Si noti che l'oggetto puo smagnetizzarsi o meno a seconda del tipo di materiale, l'acciaio per esempio resta magnetizzato.  

![magnetic_induction](https://user-images.githubusercontent.com/7195133/217617289-fcaf6a9c-0907-47d1-9007-616e58cbe312.jpg)  

Si chiama allora $\vec{B}$ il campo di **induzione magnetica**, che non e' altro che l'intensita' di campo moltiplicata per il coefficiente di permeabilita' magnetica del materiale $\mu$

$\vec{B} = \mu \cdot \vec{H}$  

Si misura in tesla $[T]$ e corrispondono a $[Wb/m^2]$. Queste grandezze magnetiche verranno chiarificate piu' avanti in dettaglio.