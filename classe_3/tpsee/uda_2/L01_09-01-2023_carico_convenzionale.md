# Carico convenzionale  

Per *dimensionare un impianto elettrico* e quindi scegliere in modo appropriato i suoi componenti, c'e' bisogno di stimare le potenze e le correnti che saranno in gioco. Purtroppo non e' possibile sapere in anticipo come l'impianto verra' utilizzato nel dettaglio, l'uso delle prese e' l'esempio piu' ovvio: quali e quanti apparecchi verranno utlitzzati ? saranno utilizzati nello stesso momento ?  

Bisogna allora necessariamente affidarci a ipotesi semplificative e coefficienti fissati con criteri statistici.  

La stima di queste grandezze si chiama **carico convenzionale** che puo' riferirsi alla potenza, o alla corrente.  


# Potenza convenzionale  

La potenza convenzionale e' la potenza attiva stimata per la quale deve essere dimensionato un impianto, che viene calcolata ogni qualvolta la potenza necessaria effettiva non e' nota. Per fare queste stime si tiene conto di due fattori principali:  

1. fattore di utilizzazione $K_u$
2. fattore di contemporaneita' $K_c$  

# Fattore di utilizzazione  

Il fattore di utilizzazione e' il rapporto tra la potenza assorbita $P_a$ e la potenza nominale $P_n$. Per esempio in un motore elettrico la potenza nominale e' la potenza resa, cioe' quella in uscita, ovvero che tiene conto di un fattore di rendimento $\eta$ (parte della potenza viene persa e.g. dissipata in calore etc...) allora sia ha che la potenza assorbita e':  

$P_n = P_a \cdot \eta$  

$P_a = \dfrac{P_n}{\eta}$  


```mermaid
flowchart LR
    in("Potenza assorbita")--->motore
    subgraph motore["&eta;"]
        A["Motore"]
    end
    motore--->out("Potenza nominale")
```

Se volessimo calcolare la potenza convenzionale di un motore elettrico di potenza nominale di $P_n = 11\ kW$ con rendimento di $\eta = 0.88$ e funzionante a $3/4$ di carico allora si avrebbe che:  

$P_a = \dfrac{P_n}{\eta} = \dfrac{11}{0.88} = 12.5\ kW$  

Trovata la potenza assorbita stimata, possiamo stimare la sua **potenza convenzionale** tenendo conto del fattore di utilizzo $K_u = \frac{3}{4} = 0.75$ ovvero:  

$P_c = P_a \cdot K_u = 12.5 \cdot 0.75 = 9.375\ W$  


# Fattore di contemporaneita'  

Il fattore di contemporaneita' ci aiuta a tenere conto del fatto che non sempre gli apparecchi vengono utilizzati tutti nello stesso momento. La potenza totale assorbita sara' in ogni caso minore o uguale alla somma delle potenze dei singoli utilizzatori.  

$P_{at} \le P_1 + P_2 + ... + P_n$

Il fattore $K_c$ e' dunque il rapporto che lega la somma delle potenze dei singoli utilizzatori con la potenza convenzionale assorbita. Si prenda per esempio un gruppo di $10$ motori da $1.5\ kW$ che solitamente non vengono utlizzati tutti nello stesso momento, quindi con un fattore $K_c = 0.6$  

$P_c = N \cdot P_a \cdot K_c = 10 \cdot 1.5 \cdot 0.6 = 15 \cdot 0.6 = 9\ kW$  

