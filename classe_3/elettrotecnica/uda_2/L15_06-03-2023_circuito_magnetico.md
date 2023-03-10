# Circuito magnetico e legge di Hopkinson  

Come si nota in figura, le linee di forza di un campo magnetico formano un circuito chiuso, questo prende il nome di **circuito magnetico**. Ci sono ovviamente linee di forza anche fuori dal nucleo magnetico, ma queste vengono ignorate per semplicita' e prendono il nome di **flusso disperso**.  

![magnetic_circuit](https://user-images.githubusercontent.com/7195133/224168072-e1f2cd06-7713-4071-a0bf-ad2bc8cdf369.jpg)  

In un certo senso, si puo' paragonare il flusso in un circuito magnetico ad una corrente di un circuito elettrico. Intuitivamente allora, a parita' di forza magnetomotrice $F_m$ o elettromotrice $V$ nel circuito elettrico, se la resistenza del circuito aumenta, allora il flusso deve diminuire.  

$\dfrac{V}{R} = I$  

$\dfrac{F_m}{R_m} = \phi$  

Questa prende il nome di **legge di Hopkinson**, dove $F_m$ e' la forza magnetomotrice mentre $R_m$ e' la **riluttanza magnetica**, ovvero l'attitudine di un corpo ad impedire il passaggio delle linee di flusso. Vogliamo ora derivare questa legge partendo dalla definizione di flusso magnetico, ricordando che $\ell a$ rappresenta in questo caso la *lunghezza di tutto il circuito*, mentre $S$ e' sempre la sezione, come $N$ il numero di spire.  

$\phi = B \cdot S = \mu \cdot H \cdot S = \mu \cdot \dfrac{NI}{\ell a} \cdot S$  

Isolando la causa del flusso, ovvero la forza magnetomotrice $F_m = NI$ si ha allora che:  

$NI = \dfrac{1}{\mu} \cdot\dfrac{\ell a}{S} \cdot \phi$  

Possiamo allora concludere che se la forza magnetomotrice $NI$ e' la causa, allora il flusso magnetico $\phi$ e' l'effetto, e quello che resta viene appunto chiamata riluttanza magnetica $\mathcal{R}$  

$\mathcal{R} = R_m = \dfrac{1}{\mu} \cdot \dfrac{\ell a}{S}$  

$\mathcal{F} = F_m = NI$  

$\mathcal{F} = \mathcal{R} \cdot \phi = \dfrac{1}{\mu} \cdot\dfrac{\ell a}{S} \cdot \phi$  

E' importante notare che dalla definizione di riluttanza si puo' dedurre il comportamento di $\mathcal{R}$ in dipendenza delle sue componeti.  

| Causa             | Effetto                |
| ----------------- | ---------------------- |
| $\ell a \uparrow$ | $\mathcal{R} \uparrow$ |
| $S \downarrow$    | $\mathcal{R} \uparrow$ |
| $\mu \downarrow$  | $\mathcal{R} \uparrow$ |

Cio' significa che a parita' di corrente $I$ nell' avvolgimento, si avra' un aumento di riluttanza quando:  

* la lunghezza del circuito aumenta
* la sezione diminuisce
* la permeabilita' diminuisce