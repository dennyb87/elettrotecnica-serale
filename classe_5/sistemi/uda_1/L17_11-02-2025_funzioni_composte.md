# Funzioni di trasferimento composte    

Dato il numero complesso $z = (a+jb) \cdot (c+jd)$ si ha che...  


$|z| = \bigg|(a+jb) \cdot (c+jd)\bigg| = \bigg|(a+jb)\bigg|\cdot\bigg|(c+jd)\bigg|$  

Formalmente...

> *Il modulo del prodotto e' uguale al prodotto dei moduli*

Percui, data una funzione di trasferimento $G(s) = s \cdot \dfrac{1}{1+\dfrac{s}{100}}$ possiamo scrivere...  

$|G| = \bigg|s \cdot \dfrac{1}{1+\dfrac{s}{100}}\bigg| = |s|\cdot\bigg|\dfrac{1}{1+\dfrac{s}{100}}\bigg|$  

In modo piu' compatto...  

$G(s) = A(s)\cdot B(s) \implies |G| = |A|\cdot|B|$  

Sostituendo alla definizione di $|G|_{db}$ e utilizzando le proprieta' dei logaritmi si ha infine che...  

$|G|_{db} = 20\log \bigg(|G|\bigg) = 20\log \bigg(|A|\cdot|B|\bigg) = 20\log|A| +20\log|B|$  

$|G|_{db} = |A|_{db}+|B|_{db}$  

## Grafico  

Conosciamo gia' il grafico del *polo di Bode*:  

$|B|_{db} = 20\log\bigg(\dfrac{1}{\sqrt{1+\dfrac{\omega^2}{100^2}}}\bigg)$  

Mentre l'altra componente e' una retta con pendenza di $20\ \frac{db}{dec}$  

$|A|_{db} = 20\log \omega$  

![composite_bode](https://github.com/user-attachments/assets/0f4cf25e-d2ff-4b2c-ad97-4af8151d2f77)    

Tracciando entrambe i grafici e sommando le rispettive ordinate in ogni punto troviamo la quindi la funzione risultante $|G|_{db}$ dove $|A|_{db}$ non e' influenzata da $|B|_{db}$ essendo zero fino a $\omega = 100\ \frac{rad}{s}$ mentre con $\omega \gt 100$ le funzioni hanno pendenza uguale ed opposta, e si annullano a vicenda risultando in una retta a pendenza zero.  
