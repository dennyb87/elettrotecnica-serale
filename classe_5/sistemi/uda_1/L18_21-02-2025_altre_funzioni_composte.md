# Altre funzioni composte  

$G(s) = \dfrac{1}{s}\cdot\dfrac{1+\dfrac{s}{100}}{1+\dfrac{s}{10}}$  

Sempre dai numeri complessi possiamo riscriverla come...  

$G(s) = \dfrac{1}{s}\cdot \bigg(1+\dfrac{s}{100}\bigg) \cdot \dfrac{1}{1+\dfrac{s}{10}} = A(s)\cdot B(s)\cdot C(s)$  

Sapendo che il modulo del prodotto e' uguale al prodotto dei moduli e utilizzando le proprieta' dei logaritmi...  

$|G|_{db} = 20\log\bigg(|A|\cdot|B|\cdot|C|\bigg) = |A|_{db}+|B|_{db}+|C|_{db}$  

Sappiamo per esperienza che $|A|_{db}$ e' una retta di pendenza $-20\ \frac{db}{dec}$ centrata in $\omega_p = 1\ \frac{rad}{s}$  

$|A|_{db} = 20\log\bigg(\dfrac{1}{\omega}\bigg)$  

Mentre sempre per esperienza sappiamo che $|B|_{db}$ e $|C|_{db}$ seguono l'ormai noto andamento e sono centrati nei rispettivi punti di singolarita'.  

![moar_complex_bode_stuff](https://github.com/user-attachments/assets/d19f51b1-bd40-4298-ac0b-83daaa70f355)  

Tracciando i grafici asintotici e sommando le ordinate delle rispettive funzioni troviamo quindi la $|G|_{db}$ risultante. Si puo' notare che $|A|_{db}$ non e' influenzata fino a $\omega = 10\ \frac{rad}{s}$ dove $|C|_{db}$ fa sentire il suo effetto facendo aumentare la pendenza fino a $-40\ \frac{db}{dec}$. Questo effetto viene pero' annullato da $|B|_{db}$ quando $\omega = 100\ \frac{rad}{s}$ riportando la pendenza a $-20\ \frac{db}{dec}$.  
