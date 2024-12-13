# Rifasamento  

![load_over_time](https://github.com/user-attachments/assets/4f758390-3381-4585-8a0c-c03d56e7bc31)  

Ai fini dell'efficienza energetica, ma piu' spesso per soddisfare le condizioni del distributore di energia, e necessario installare delle batterie di rifasamento. Questa operazione permette a parita' di potenza attiva $P$ di far funzionare l'impianto con corrente minore.  

Si consideri una situazione in cui il carico varia nel tempo con un andamento di questo tipo...  


|     | $P[kW]$ | $\cos\varphi$ |
| --- | ------- | ------------- |
| 1   | $140$   | $0.8$         |
| 2   | $60$    | $0.6$         |
| 3   | $100$   | $0.5$         |

Ricordando la formula generale per la potenza reattiva di rifasamento:  

$Q_r = P\cdot(\tan\varphi_0-\tan\varphi_r)$  

Dove $\varphi_0$ e' l'angolo orginale mentre $\varphi_r$ e' l'angolo desiderato dopo il rifasamento. Procediamo a calcolare le potenze reattive di rifasamento dei rispettivi carichi ipotizzando $\cos\varphi_r = 0.95$  

$Q_{r1} = P_1(\tan\varphi_1-\tan\varphi_r)=140(0.75-0.329)= 58.94\ \text{kVAR}$  

$Q_{r2} = P_2(\tan\varphi_2-\tan\varphi_r)=60(1.33-0.329)\simeq 60\ \text{kVAR}$  

$Q_{r3} = P_3(\tan\varphi_3-\tan\varphi_r)=100(1.73-0.329)\simeq 140\ \text{kVAR}$  

Considerata una potenza reattiva massima di $140\ \text{kVAR}$ si sceglie dalle tabelle a pagina **X-214/218** il regolatore automatico con batterie a gradini da $150$ a 9 combinazioni. In questo modo potremo configurare due moduli $30+30$ per $Q_{r1}/Q_{r2}$ mentre utilizzare tutti i moduli, per un totale di $150$ per $Q_{r3}$. La potenza in eccesso di $Q_{r3}$ in realta' ci permette di ottenere un angolo di rifasamento maggiore.  

$150 = 100\cdot(1.73-\tan\varphi_r) = 173 - 100\tan\varphi_r \implies \tan\varphi_r = \dfrac{173-150}{100} = 0.23$  

$\tan\varphi_r = 0.23 \implies \cos\varphi_r \simeq 0.97$  

E' importante notare che prima del rifasamento al tempo $t_3$ la corrente era...   

$I = \dfrac{P}{\sqrt{3}\cdot V\cdot\cos\varphi_0} = \dfrac{100\ 000}{\sqrt{3}\cdot 400\cdot 0.5} \simeq 289\ A$  

Mentre dopo il rifasamento si ha che...  

$I = \dfrac{P}{\sqrt{3}\cdot V\cdot\cos\varphi_r} = \dfrac{100\ 000}{\sqrt{3}\cdot 400\cdot 0.97} \simeq 149\ A$  

