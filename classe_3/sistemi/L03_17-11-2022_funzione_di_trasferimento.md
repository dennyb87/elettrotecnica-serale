# Funzione di trasferimento  

Un sistema puo e' essere guardato da diversi punti di vista, prendiamo  
per esempio un distributore di benzina.
Dal punto di vista del consumatore il distributore e' un sistema che  
accetta denaro come input, ed eroga benzina come output.  
Dal punto di vista del gestore pero' le cose cambiano.  

## Vista consumatore

```mermaid
flowchart LR
    in("denaro")--"input"--->sistema
    subgraph sistema[ ]
        A["distributore"]
    end
    sistema--"output"--->out("benzina")
```

## Vista gestore

```mermaid
flowchart LR
    in("benzina")--"input"--->sistema
    subgraph sistema[ ]
        A["distributore"]
    end
    sistema--"output"--->out("denaro")
```  

Si capisce quindi che la descrizione del sistema puo' cambiare a  
seconda del punto da cui lo si osserva.  
Per il momento prendiamo in considerazione solo il punto di vista del  
consumatore.  

$sistema = distributore_{vistaconsumatore}$  

Supponiamo che prezzo il della benzina sia di $2\ \epsilon/\ell$  
Dopo qualche rifornimento si avrebbe questa tabella.  

| $\epsilon$ | $\ell$ | $\epsilon/\ell$ |
| ---------- | ------ | --------------- |
| $5$        | $2.5$  | $\frac{1}{2}$   |
| $10$       | $5$    | $\frac{1}{2}$   |
| $15$       | $7.5$  | $\frac{1}{2}$   |


Il rapporto tra output ed input prende il nome di **funzione di trasferimento**  
e si indica con $F$.  
$F = \frac{y}{x} = \frac{output}{input}$  

Nel nostro esempio abbiamo quindi $F = \frac{\ell}{\epsilon}$  ovvero $\ell = F \cdot \epsilon$  
Dato che $F = \frac{1}{2}$ allora $\frac{1}{2} \cdot \epsilon = \ell$

Il nome **funzione di trasferimento** viene proprio dal fatto che permette  
di trasformare l'input in output.  

$F \cdot input = output$  


# Funzione di trasferimento piatto rotante microonde  

In tabella si ha il tempo $t$ in secondi impiegato per completare  
$n$ giri del piatto rotante all'interno di un microonde.  
L'ultima colonna rappresenta la **funzione di traserimento**.

| $t$  | $n$ | $n/t$          |
| ---- | --- | -------------- |
| $25$ | $1$ | $\frac{1}{25}$ |
| $50$ | $2$ | $\frac{1}{25}$ |
| $75$ | $3$ | $\frac{1}{25}$ |