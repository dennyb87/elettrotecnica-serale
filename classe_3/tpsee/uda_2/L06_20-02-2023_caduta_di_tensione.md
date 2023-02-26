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

Calcoliamo ora la portata supponendo di non dover necessariamente supportare $16\ A$.  

![posa_4](https://user-images.githubusercontent.com/7195133/221414018-636cce15-b258-4b5e-8cc1-6f02baf05f4d.jpg)  

Per un circuito monofase, quindi 2 conduttori caricati, isolati in **PVC** potrebbe essere appropriata una sezione da $1.5\ mm^2$ quindi $I_0 = 17.5\ A$.  

![correzione_k2](https://user-images.githubusercontent.com/7195133/221414203-e2da581b-68e9-4f2b-b08f-630494cd40c3.jpg)  

Si utlizza un $K_1$ unitario, mentre un fattore $K_2 = 0.65$ in quanto stiamo posando un circuito in una canala con 3 circuiti gia' presenti.  

$I_z = I_0 \cdot K_1 \cdot K_2 = 17.5 \cdot 0.65 = 11.375\ A$  

Questa portata soddisferebbe in teoria la condizione $I_b \le I_z$  ovvero $9.6 \le 11.375$. 

## Metodo della caduta di tensione unitaria

Supponiamo ora una caduta massima del 2% ovvero:  

$\Delta V = \dfrac{\Delta V_{pc} \cdot V_n}{100} = \dfrac{2 \cdot 230}{100} = 4.6\ V$  

Utilizziamo quindi il metodo per il calcolo della caduta di tensione unitaria.    

$u = \dfrac{\Delta V \cdot 1000}{I_b \cdot L} = \dfrac{4.6 \cdot 1000}{9.6 \cdot 50} \simeq 9.58\ \frac{mV}{Am}$    

![cadute_tensione_unitarie](https://user-images.githubusercontent.com/7195133/221426936-89e77f33-8603-42f3-86c9-f624d54dafff.jpg)

Vediamo allora che stimando per esempio un $\cos \varphi\ 0.8$, per i nostri cavi unipolari monofase $50\ m$ ci serve quindi una sezione di $4\ mm^2$ in quanto e' quella che piu' si avvicina alla caduta unitaria calcolata $9.58 \simeq 9.08$. I $2\ mm^2$ ricavati dal calcolo della portata, pur supportando la corrente di impiego, non sono sufficienti per ottenere una caduta massima di $4.6\ V$.