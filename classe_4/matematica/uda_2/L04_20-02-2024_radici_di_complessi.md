# Radici di numeri complessi  

Proviamo a trovare la radici cubiche di $z^3 = 1$ ovvero si vuole risolvere per $z$  

$z^3 - 1 = 0$  

Questa e' una differenza di cubi, per cui...  

$(\underbrace{z -1}_{z_0 = 1})(z^2+z+1) = 0$  

Utilizziamo la quadratica per $z^2+z+1$  

$z = \dfrac{-1\pm\sqrt{1-4}}{2} = \dfrac{-1\pm\sqrt{3}i}{2}$  

$z_1 = -\frac{1}{2} + \frac{\sqrt{3}}{2}i$  

$z_2 = -\frac{1}{2} + \frac{\sqrt{3}}{2} i$  

Abbiamo trovato tre soluzioni che una volta riportate sul piano di Gauss scorpiamo essere equidistanti in termini di angoli.  

![cube_root_example](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/a2978120-b8d2-471e-97cd-293642e02e05)  

In generale troviamo che $\sqrt[^n]{z}$ da sempre $n$ soluzioni, ma per casi piu' complessi diventa sconveniente risolvere in forma algebrica, per cui si vuole trovare una formula generale. Supponiamo di avere un numero complesso:  

$z = r(\cos \theta+i\sin\theta)$  

Le sue radici $n$ devono essere...  

$\sqrt[^n]{z} = \sqrt[^n]{r(\cos \theta +i\sin \theta)} = r^{\frac{1}{n}}(\cos \theta +i\sin \theta)^{\frac{1}{n}}$  

Per il teorema di *De Moivre*...  

$\sqrt[^n]{r} \cdot (\cos \frac{\theta}{n} +i\sin \frac{\theta}{n})$  

Questa forma e' pero' incompleta in quanto non ci permette di trovare tutte le soluzioni. E' dimostrabile che la formula per trovare gli angoli di interesse e' descrivibile con $\alpha = \dfrac{2\pi k}{n}$ per cui si ha infine che...  

$\sqrt[^n]{z} = \sqrt[^n]{r} \cdot (\cos \frac{2\pi k +\theta}{n} +i\sin \frac{2\pi k +\theta}{n})$  

Con $k$ che va da $0 \to n-1$  
