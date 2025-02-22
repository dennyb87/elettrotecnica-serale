# Polo di Bode  

$G(s) = \dfrac{1}{1+\dfrac{s}{100}}$  

In questo sistema si ha un polo negativo $p = -100$ e di conseguenza una singolarita' in $\omega_p = 100\ \frac{rad}{s}$ che ci aiutera' a centrare il grafico di $|G|_{db}$ dopo aver trovato il modulo e la fase...  

## Modulo  

$|G| = \dfrac{1}{\sqrt{1+\dfrac{\omega^2}{100^2}}}$  

Esaminiamo i limiti particolari...  

$\displaystyle{\lim_{\omega\to 0}}\ |G| = \dfrac{1}{\sqrt{1+\dfrac{0^2}{100^2}}} = 1$  

$\displaystyle{\lim_{\omega\to 100}}\ |G| = \dfrac{1}{\sqrt{1+\dfrac{100^2}{100^2}}} = \dfrac{1}{\sqrt{2}} = \dfrac{\sqrt{2}}{2}$  

$\displaystyle{\lim_{\omega\to \infty}}\ |G| = \dfrac{1}{\sqrt{1+\dfrac{\omega^2}{100^2}}} = \dfrac{1}{\dfrac{\omega}{100}\cdot\sqrt{\dfrac{100^2}{\omega^2}+1}} =  \dfrac{100}{\omega}$  

Troviamo quindi alcuni valori chiave in $db$ ...  

$|G(0)|_{db} = 20\log(1) = 0\ db$  

$|G(100)|_{db} = 20\log(\frac{\sqrt{2}}{2}) \simeq -3\ db$  

$|G(10\ 000)|_{db} = 20\log(\frac{100}{10\ 000}) = -40\ db$  

![polo_di_bode](https://github.com/user-attachments/assets/7c57e0ef-854b-4e8f-9624-c24def1e0a72)  

Tracciando il grafico notiamo allora che la funzione comincia a diventare negativa proprio quando $\omega \simeq 100\ \frac{rad}{s}$ e per semplicita' disegneremo sempre il grafico asintotico ignorando quindi la curva reale smussata. E' possibile quindi tracciare il grafico senza fare troppi calcoli sapendo che la funzione ha valore zero fino al punti di singolarita' alla velocita' angolare di taglio $\omega_p$ in cui centriamo il grafico, dopodiche' si ha una pendenza di $-20\ \frac{db}{dec}$

## Fase  

Per trovare il grafico della fase, ricordiamo che l'angolo di un numero complesso $z = a+jb$ e' individuato da...  

$\theta_z = \arctan \bigg(\dfrac{b}{a}\bigg)$  

Nel nostro caso abbiamo:  

$G(jw) = \dfrac{1}{1+\dfrac{j\omega}{100}}$  

Ricordando che la fase del quoziente di due numeri complessi e' la differenza delle fasi, troviamo prima le rispettive fasi del numeratore $N$ e del denominatore $D$...  

$N = 1+j0 \implies \theta_N = \arctan\bigg(\dfrac{0}{1}\bigg) = 0^\circ$  

$D = 1+j\frac{\omega}{100} \implies \theta_D = \arctan\bigg(\dfrac{\omega}{100}\bigg)$  

Allora...  

$\angle G = \theta_N - \theta_D = 0^\circ - \arctan\bigg(\dfrac{\omega}{100}\bigg)$  

Esaminando i limiti particolari...  

$\displaystyle{\lim_{\omega\to 0}}\ \angle G = 0^\circ - \arctan\bigg(\dfrac{0}{100}\bigg) = 0^\circ - 0^\circ = 0^\circ$  

$\displaystyle{\lim_{\omega\to 0}}\ \angle G = 0^\circ - \arctan\bigg(\dfrac{100}{100}\bigg) = 0^\circ - 45^\circ=-45^\circ$  

$\displaystyle{\lim_{\omega\to +\infty}}\ \angle G = 0^\circ - \arctan\bigg(\dfrac{+\infty}{100}\bigg) = 0^\circ - 90^\circ = -90^\circ$  

![polo_di_bode_fase](https://github.com/user-attachments/assets/b92f271b-1890-484f-98d9-b9954ff2b27b)  

Tracciando il grafico scopriamo allora che la funzione e' parte da zero e comincia a decrescere una decade prima del punto di singolarita' $\omega = 100\ \frac{rad}{s}$ con una pendenza di $-45\ \frac{\circ}{dec}$ stabilizzandosi definitivamente la decade successiva a $-90\ \frac{\circ}{dec}$  
