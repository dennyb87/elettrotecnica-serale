# Prodotti, quozienti e potenze di numeri complessi  

Sappiamo che dato un numero complesso in forma polare e' possile trovare la sua forma trigonometriga.  

$z(|z|, \theta) \implies z = |z|\cos\theta + i|z|\sin\theta= |z|(\cos\theta + i\sin\theta)$  

Date le forme trigonometriche di due numeri complessi $z_1, z_2$ e' dimostrabile che il loro **prodotto** equivale a:  

$z_1 \cdot z_2 = |z_1||z_2|(\cos(\alpha+\beta)+i\sin(\alpha+\beta))$  

Si ha che il loro **quoziente** e' invece:  

$\dfrac{z_1}{z_2} = \dfrac{|z_1|}{|z_2|}(\cos(\alpha-\beta)+i\sin(\alpha-\beta))$  

Infine si puo' dimostrare che un numero complesso $z$ elevato alla **potenza** $n$ equivale a:  

$z^n = |z|^n(\cos n \cdot\theta + i\sin n \cdot \theta)$  


## Dimostrazione del prodotto  

$z_1 = |z_1|(\cos\alpha+i\sin\alpha)$  
$z_2 = |z_2|(\cos\beta+i\sin\beta)$  

$z_1 \cdot z_2 = |z_1|(\cos\alpha+i\sin\alpha) \cdot |z_2|(\cos\beta+i\sin\beta)$  

$z_1 \cdot z_2 = |z_1||z_2| \cdot (\cos\alpha+i\sin\alpha)(\cos\beta+i\sin\beta)$  

$z_1 \cdot z_2 = |z_1||z_2| \cdot (\cos\alpha\cos\beta + i\cos\alpha\sin\beta + i\cos\beta\sin\alpha +i^2\sin\alpha\sin\beta)$  

$z_1 \cdot z_2 = |z_1||z_2| \cdot (\cos\alpha\cos\beta + i\cos\alpha\sin\beta + i\cos\beta\sin\alpha -\sin\alpha\sin\beta)$  

$z_1 \cdot z_2 = |z_1||z_2| \cdot (\underbrace{\cos\alpha\cos\beta -\sin\alpha\sin\beta}_{identita\ trigononometriche} + i(\underbrace{\cos\alpha\sin\beta + \cos\beta\sin\alpha}))$  

Allora semplifichiamo utilizzando le *identita' trigonometriche* trovando infine...  

$z_1 \cdot z_2 = |z_1||z_2|(\cos(\alpha+\beta)+i\sin(\alpha+\beta))$  

## Dimostrazione della potenza con il teorema di De Moivre  

L'elevamento a potenza ci dice che:  

$z^n = |z|^n \cdot (\cos \theta + i\sin \theta)^n = |z|^n(\cos n \theta + i\sin n\theta)$  

Ma questo implica che...  

$(\cos \theta + i\sin \theta)^n = \cos n\theta + i\sin n\theta$

Questo passaggio e' il teorema di *De Moivre* dimostrabile per induzione. Iniziamo con la base di induzione con $n = 0$  

$(\cos \theta + i\sin \theta)^0 = \cos 0\theta + i\sin 0\theta = 1 + 0i =1\ \ \checkmark$  

Se e' vero per $n = 0$ si **assume** allora che sia vero anche per un generico $k$  

$(\cos \theta + i\sin \theta)^k = \cos k\theta + i\sin k\theta$  

Procediamo quindi alla dimostrazione che sia vero anche per $k+1$  

$(\cos \theta + i\sin \theta)^{k+1} = \cos \bigg[(k+1)\theta \bigg]+ i\sin \bigg[(k+1)\theta\bigg]$  

Si procede ad espandere il primo membro...  

$(\cos \theta + i\sin \theta)^{k+1}$  

$(\cos \theta + i\sin \theta)^1(\cos \theta + i\sin \theta)^k$  

$(\cos \theta + i\sin \theta)\underbrace{\bigg[\cos k\theta + i\sin k\theta\bigg]}_{per\ assunzione}$  

$\cos \theta \cos k\theta + i\cos \theta \sin k\theta +i\sin \theta \cos k\theta + i^2 \sin\theta \sin k\theta$  

$\cos \theta \cos k\theta - \sin\theta \sin k\theta + i\bigg[\cos \theta \sin k\theta +\sin \theta \cos k\theta\bigg]$  

Dalle identita' trigonometriche si dimostra infine che in effetti il primo membro e' uguale al secondo per $k+1$  

$\cos \bigg[\theta + k\theta\bigg] + i\sin\bigg[\theta + k\theta\bigg]$  

$\cos \bigg[(k+1)\theta \bigg]+ i\sin \bigg[(k+1)\theta\bigg]$  
