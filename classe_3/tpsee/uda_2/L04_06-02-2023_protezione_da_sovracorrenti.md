# Protezione da sovracorrenti  

Quando dimensioniamo un impianto dobbiamo assicurarci di proteggerlo dalle sovracorrenti, queste possono essere causate da un **sovraccarico** o da un **corto circuito**. Entrambe indicano la presenza di una grande corrente, la differenza e' che il **sovraccarico** identifica quella che scorre in un **circuito sano**, mentre il corto circuito quella che scorre in un **circuito guasto**.  

Per proteggersi dalle sovracorrenti bisogna assicurarsi che la portada $I_z$ dei cavi sia maggiore o uguale alla corrente di intervento $I_n$ del sistema di protezione e.g. un magnetotermico, e che quella del sistema di protezione sia a sua volta maggior o uguale a quella della corrente di impiego $I_b$ stimata.  

$I_b \le I_n \le I_z$  

Che questo sia necessario diventa evidente se proviamo a pensare a cosa potrebbe succedere nel caso in cui questa disequazione fosse falsa. Poniamo per assurdo $I_z < I_n$ quindi con la portata minore del magnetotermico, allora il magnetotermico entrerebbe in azione solo dopo che il cavo abbia superato la sua portata con potenziali danni all'isolante e all'impianto stesso. Se invece ponessimo $I_n < I_b$ va da se che non potremmo utilizzare l'impianto perche' il magnetotermico ce lo impedirebbe visto che la sua soglia di intervento sarebbe minore della corrente di impiego.  

## Simulazione  

Prendiamo in considerazione un gruppo di $4$ prese da $16\ A$ su un impianto ad una tensione di $V_n = 230\ V$ ed un $\cos \varphi = 0.9$. Calcoliamo allora la potenza convenzionale $P_c$ e la corrente di impiego $I_b$ con un coefficiente di riduzione di $0.1$      

$P_c = 4 \cdot 16 \cdot 230 \cdot 0.9 \cdot 0.1 = 1324.8\ W$  

$I_b = \dfrac{P_c}{V_n \cdot \cos \varphi} = \dfrac{1324.8}{230 \cdot 0.9} = 6.4\ A$  

Supponendo una posa con cavo in aria libera in strato a soffitto, ovvero la posa $11A$ e considerata una temperatura di $30\degree$ quindi un coefficitente $K_1 = 1$ mentre un coefficiente di posa $K_2 = 0.9$ possiamo allora calcolare la portata dei cavi ricondandoci che $I_z \ge I_b$  

$I_z = I_0 \cdot K_1 \cdot K_2 = I_0 \cdot 1 \cdot 0.9 = I_0 \cdot 0.9$  

$I_z \cdot 0.9 \ge 6.4\ A \implies I_z \ge \dfrac{6.4}{0.9} \implies I_z \ge 7.1\ A$  

Questo significa che la portata minima dovra' essere maggiore o uguale a $7.1\ A$.  

Certo abbiamo trovato potenza convenzionale, la corrente di impiego, e la portata minima, ma le prese sono da $16\ A$ e queste non si possono ignorare. Si deve allora supportare almeno la portata delle prese, e quindi installare un magnetotermico da $16\ A$ che permetta di sfruttare al massimo le prese, percio' va da se che anche la portata dei cavi dovra' supportare tale corrente.  

Per trovare la sezione del cavo andiamo a calcolare la portata con diverse sezioni.  

$S_1 = 1\ mm^2 \implies I_1 = 13.5\ A$  
$S_2 = 1.5\ mm^2 \implies I_2 = 17.5\ A$  
$S_3 = 2.5\ mm^2 \implies I_3 = 24\ A$  

$I_{z1} = I_1 \cdot 0.9 = 13.5 \cdot 0.9 = 12.15\ A$  
$I_{z2} = I_2 \cdot 0.9 = 17.5 \cdot 0.9 = 15.75\ A$  
$I_{z3} = I_3 \cdot 0.9 = 24 \cdot 0.9 = 21.6\ A$  

Sceglieremo allora una sezione di $2.5\ mm^2$ in quanto permette una portata che supporta le prese e soprattutto e' maggiore del magnetotermico.