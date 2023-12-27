# Teorema del coseno  

Il teorema del coseno ci permette di calcolare i lati di un triangolo qualsiasi conoscendo gli altri due, e il coseno dell'angolo tra di loro.  

![law_of_cosines](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/16f94808-31b6-48ef-88eb-74890b350ee4)  

Tracciando l'altezza $h$ possiamo scrivere che...  

$a^2 = h^2 + DC^2$  

Sappiamo che $DC = b - AD$ e che $AD = c \cdot \cos \alpha$ allora...  

$DC = b - c \cdot \cos \alpha$  

Sostituiamo...  

$a^2 = h^2 + (b - c \cdot \cos \alpha)^2$  

Sappiamo anche che $h = c \cdot \sin \alpha$ percui...  

$a^2 = (c \cdot \sin \alpha)^2 + (b - c \cdot \cos \alpha)^2$  

Sviluppiamo i quadrati...  

$a^2 = \underbrace{c^2 \cdot \sin^2 \alpha} + b^2 + \underbrace{c^2 \cdot \cos^2 \alpha} - 2bc \cdot \cos \alpha$  

$a^2 = c^2 \cdot(\sin^2 \alpha + \cos^2 \alpha) + b^2 - 2bc \cdot \cos \alpha$  

$a^2 = c^2 \cdot 1 + b^2 - 2bc \cdot \cos \alpha$  

Si ha infine che...  

$a^2 = c^2 + b^2 - 2bc \cdot \cos \alpha$  
