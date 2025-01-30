# Scorrimento  

Nel motore asincrono il campo magnetico rotante ruota nello stesso senso del rotore a meno che non vengano invertite le fasi (ad esempio per un inversione di marcia). E' importante notare pero' che nel momento in cui il rotore raggiunge la stessa velocita' del campo induttore non si ha nessuna variazione di flusso e di conseguenza nessuna coppia motrice. Per questo motivo il rotore e' costretto ad una velocita' di rotazione minore. Il rapporto tra questa differenza di velocita' e la velocita' del campo induttore prende il nome di **scorrimento** (*slip*), e spiega il motivo per cui viene chiamato **motore asincrono**.  

$s = \dfrac{n_0-n}{n_0}$  

Dove $n_0$ e' la velocita' del campo induttore, mentre $n$ e' quella dello statore. Indicativamente si puo' avere uno scorrimento intorno al 3%. Dato un motore alimentato a $f = 50\ Hz$ con 6 poli magnetici, ovvero 3 coppie polari $P$ si ha che:  

$2P = 6 \implies P = \frac{6}{2} = 3$  

$n_0 = \dfrac{60f}{P} = \dfrac{60\cdot 50}{3} = 1000\ \text{rpm}$  

Se il rotore ha una velocita' di $970\ \text{rpm}$ allora lo scorrimento sara'...    

$s = \dfrac{n_0-n}{n_0} = \dfrac{1000-970}{1000} = 0.03$  

Quindi proprio uno scorrimento del 3%.
Infine e' importante notare che se $n = 0$ il rotore e' fermo percio' $s = 1$. Se invece $s = 0$ allora $n_0 = n$ ovvero rotore e campo induttore sono sincronizzati.  

## Tensioni indotte  

$E_1 = K_1\cdot N_1\cdot f\cdot\phi$  

Questa e' la **tensione indotta** in **fase statorica**, ovvero la tensione generata negli avvolgimenti statorici a causa della variazione di flusso. Dove $K_1$ dipende dalla geometria, materiali e numero di poli dello statore, $N_1$ e' il numero di spire degli avvolgimenti, $f$ e' la frequenza, mentre $\phi$ e' il flusso magnetico.  

$E_2 = K_2\cdot N_2\cdot f_r\cdot \phi$  

Mentre la **tensione indotta** in **fase rotorica**, ovvero la tensione generata nel rotore a causa della variazione di flusso. Questa dipende, oltre che dalla geometria e numero di spire, dalla frequenza rotorica $f_r$ che e' molto minore di quella del campo induttore $f$ in quanto dipende dallo scorrimento $s$ in particolare si ha che:  

$f_r = s\cdot f$  

Si ha allora che a rotore fermo (o bloccato) $f_r = f$ percio' viene definita:  

$E_{20} = \dfrac{E_2}{s} = K_2\cdot N_2\cdot f\cdot \phi \implies E_2 = s\cdot E_{20}$  

Percio' dall'esempio sullo scorrimento si ha che:  

$f_r = 0.03\cdot 50 = 1.5\ Hz$  

Il [rotore rincorre il campo magnetico rotante](https://youtu.be/AQqyGNOP_3o?si=Bv3rBbfOhP-lJ2wQ&t=166) senza raggiungerlo con uno scorrimento del 3%, percio' il campo induttore vede una variazione di flusso relativa piuttosto piccola che porta quindi ad una piccola una frequenza rotorica. Essendo una frequenza molto bassa, sul rotore non si tiene conto delle perdite nel ferro che dipendendo appunto dalla frequenza sono quindi tracurabili.  

# Circuito equivalente  

![circuito_equivalente_2](https://github.com/user-attachments/assets/f3e2f90e-f1fd-4326-a207-de8adc8d5109)   

Il circuito equivalente e' analogo a quello di un trasformatore. Dove $V_1$ e' la tensione di alimentazione, $E_1$ la tensione in fase statorica, $E_2$ la tensione in fase rotorica. A questo punto abbiamo un circuito equivalente che sul lato del rotore ha una resistenza costante ed una reattanza variabile dipendente da $s$. Vogliamo a questo punto manipolare il circuito, ricordando che...  

$I_2 = \dfrac{s\cdot E_{20}}{R_2+jsX_2}$  

Dividiamo numeratore e denominatore per $s$...  

$I_2 = \dfrac{E_{20}}{\dfrac{R_2}{s}+jX_2}$  

Ma se...  

$\dfrac{R_2}{s} = \dfrac{R_2}{s}+R_2-R_2 = R_2+R_2\bigg(\dfrac{1}{s}-1\bigg)$  

Allora...  

$I_2 = \dfrac{E_{20}}{R_2+R_2\bigg(\dfrac{1}{s}-1\bigg)+jX_2}$  

Possiamo quindi riarrangiare il circuito per ottenere una resistenza variable fittizia che rappresenta il carico meccanico ovvero:  

$R_2\cdot\bigg(\dfrac{1}{s}-1\bigg)$  

![rotor_equivalent](https://github.com/user-attachments/assets/aef181d4-755c-48e6-8511-a037ce0b503b)  
