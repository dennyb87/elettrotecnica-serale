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
