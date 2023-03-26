# Oscilloscopio  

L'oscilloscopio e' uno strumento che permette di misurare e di visualizzare una grandezza fisica nel tempo, solitamente una tensione.  

![oscilloscope_controls_1](https://user-images.githubusercontent.com/7195133/227784901-9d77dbcb-9b83-4d64-8db6-6a8a01007cac.jpg)  

Come abbiamo gia' visto si presenta con una serie di controlli che permettono di variare il modo in cui il segnale viene mostrato a schermo. Il segnale quindi non viene modificato in alcun modo, e' vista sul segnale stesso che viene alterata, per esempio grazie alle unita' di misura delle divisioni temporali o della tensione. Andiamo ora ad esaminare un segnale sinusoidale.  

## Sinusoide  

![sine_wave_phasor](https://user-images.githubusercontent.com/7195133/227787960-d96bb4a0-43a4-4765-88fd-fb5ddd7ba730.gif)  

La sinusoide non e' altro che la coordinata verticale nel tempo di un vettore rotante. Questo coincide anche con il seno del triangolo rettangolo la cui ipotenusa e' il raggio di una circonferenza unitaria.  

![valore_efficace](https://user-images.githubusercontent.com/7195133/227790988-18a37f89-d3ee-4f4e-bd30-72d3ea5c75eb.jpg)  

Si ha quindi un'ampiezza massima, o picco massimo $A_{max} = V_{p^+} = V_{max}$ che coincide con il picco minimo $A_{min} = V_{p^-} = V_{min}$ ed un valore picco-picco $V_{pp}$.  

Il valore efficace $V_{eff}$ e' invece quel valore che a parita' di carico produrrebbe gli stessi effetti termici, meccanici, o luminosi di un valore continuo.  

$V_{eff} = \dfrac{V_{max}}{\sqrt{2}}$  

$V_{max} = V_{eff} \cdot \sqrt{2} = 230 \cdot 1.42 \simeq 325.27\ V$  

Quando parliamo di $230\ V$ stiamo parlando del valore efficace, il valore di picco e' in effetti circa $325.27\ V$.  

![period_and_frequency](https://user-images.githubusercontent.com/7195133/227790781-334ec1f4-5ea9-44a2-88f3-a034ed0a7940.jpg)

Il tempo impiegato per completare la circonferenza, o ciclo, viene chiamato **periodo**, ed e' l'inverso della **frequenza**, ovvero i cicli completati al secondo. Se si hanno $4\ Hz$ ovvero 4 cicli al secondo, significa che il periodo, ovvero il tempo in cui un ciclo viene completato e' di $\frac{1}{4}$ di secondo.  