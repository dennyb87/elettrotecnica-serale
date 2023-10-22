# Seno e coseno  

![sine_cosine](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/ef9fd2ec-5bea-4fdd-a60e-8917fc27df88)   

Tracciando un segmento $\overline{OP}$ nel **primo quadrante** otteniamo un angolo $\theta$ che avra' un lato adiacente $a$, un lato opposto $o$, e l'ipotenusa $h$. Per definizione il **seno** ed il **coseno** di $\theta$ sono:  

$\sin\theta = \dfrac{opposto}{ipotenusa} = \dfrac{o}{h}$  

$\cos\theta = \dfrac{adiacente}{ipotenusa} = \dfrac{a}{h}$  

Allora trovandoci in un cerchio di raggio unitario si ha che $h = 1$ per cui seno e coseno di $\theta$ saranno le rispettive coordinate $y, x$ del punto $P$.  

$\sin\theta = \dfrac{o}{1} = o = y_P$  

$\cos\theta = \dfrac{a}{1} = a = x_P$  

Questa definizione pero' non e' sufficiente per angoli maggiori di $90^\circ$ per cui si utilizzano gli **angoli supplementari** per scoprire che:  

$\sin \theta = \sin (\pi - \alpha) = \sin \alpha$  
$\cos \theta = \cos (\pi - \alpha) = - \cos \alpha$  

![supplementary_angles](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c76713f3-0d08-45bb-83c0-4813fa27cf9b)  

La nuova definizione e' quindi in accordo con la prima, riaffermando che seno e coseno di $\theta$ continuano ad essere le rispettive coordinate $y, x$ del punto $P$.  

# Triangoli rettangoli particolari  

![special_right_triangles](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f1176371-be93-4242-911e-5a00f3e3c0fe)  

Il triangolo rettangolo di $45^\circ$ ha due angoli uguali cosi' come due lati uguali, per cui dal teorema di Pitagora si ha che:  

$\sin 45^\circ = \cos 45^\circ = \dfrac{\sqrt{2}}{2}$  

Quello di $60^\circ$ se protratto nel suo riflesso forma un triangolo equilatero unitario con angoli di $60^\circ$ per cui, sempre per il teorema di Pitagora troviamo che:  

$\sin 60^\circ = \dfrac{\sqrt{3}}{2}$  

$\cos 60^\circ = \dfrac{1}{2}$  

Infine se l'angolo e' di $30^\circ$ otteniamo gli stessi risultati ma invertiti.  

$\sin 30^\circ = \dfrac{1}{2}$  

$\cos 30^\circ = \dfrac{\sqrt{3}}{2}$  

# Tangente  

![tangente](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/9294fccc-1a12-4194-91f5-03cd5b8e4e59)  

I triangoli $\overline{OAD}$ e $\overline{OCB}$ sono simili, per cui se la tangente e' definita come $\dfrac{\sin \theta}{\cos \theta}$ essendo in un cerchio unitario $\overline{OB} = 1$ si ha che la tangente coincide con $\overline{CB}$.  

$\dfrac{\sin \theta}{\cos \theta} = \dfrac{\overline{CB}}{\overline{OB}} = \dfrac{\tan \theta}{1} = \tan \theta$  

E' importante notare che $\tan$ e' una funzione periodica, come $\sin$ e $\cos$, ma non e' una funzione continua in quanto non e' definita' per angoli di $90^\circ$. Con $\theta = 90^\circ$ si avrebbe infatti:  

$\tan 90^\circ = \dfrac{\sin 90^\circ}{\cos 90^\circ} = \dfrac{1}{0} = \nexists$  