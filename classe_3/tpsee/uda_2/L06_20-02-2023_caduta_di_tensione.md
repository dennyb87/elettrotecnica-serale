# Caduta di tensione  

La **caduta di tensione**, che per un impianto si calcola dal contatore, e' *proporzionale alla lunghezza del conduttore*. La normativa ci dice che nel punto piu' sfavorevole, questa caduta deve essere minore o uguale al 4%.  

$\Delta V_{pc} \le 4_{pc}$  

Questo significa che in un impianto alimentanto a $230\ V$ e' ammissibile una caduta massima di $9.2\ V$.  

$\Delta V = \dfrac{\Delta V_{pc} \cdot V_n}{100} = \dfrac{4 \cdot 230}{100} = 9.2\ V$  

## Simulazione  

Cerchiamo ora di determinare la sezione dei cavi isolati in **PVC** di lunghezza $50\ m$ di un circuito monofase posato insieme ad altri 3 circuiti monofase gia' presenti. Supponiamo una posa $4$ a parete con canala in **PVC** e che il circuito debba alimentare $3$ prese da $16\ A$. Teniamo ora presente che bisogna soddisfare le condizioni:  

$I_b \le I_z$  

$\Delta V \le \Delta V_{max}$  

Calcoliamo allora la potenza convenzionale supponendo $\cos \varphi = 0.9$ ed un $K_p = 0.2$  

$P_c = N \cdot V_n \cdot I_{max} \cdot \cos \varphi \cdot K_p = 3 \cdot 230 \cdot 16 \cdot 0.9 \cdot 0.2 = 1987.2\ W$  

$I_b = \dfrac{P_c}{V_n \cdot \cos \varphi} = \dfrac{1987.2}{230 \cdot 0.9} = 9.6\ A$  

