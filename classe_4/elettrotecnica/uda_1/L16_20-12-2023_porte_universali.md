# Porte universali  

Dai teoremi di De Morgan e' possibile dimostrare che tutte le funzioni logiche possono essere realizzate utilizzando solo porte **NAND** o solo porte **NOR**, dette appunto **porte universali**.  

## Porta NOT  

Vogliamo derivare la porta **NOT** dal secondo teorema di De Morgan in modo da poterla riutilizzare per le altre porte in seguito:  

$\overline{A \cdot B} = \overline{A} + \overline{B} \implies \overline{A \cdot A} = \overline{A} + \overline{A} = \overline{A}$  

Se $\overline{A} = \overline{A \cdot A}$  allora e' possibile costruire una porta **NOT** utilizzando una porta **NAND**.  

![universal_nand_not](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/01730080-0b2d-492f-b746-0deb307142b5)  

## Porta OR  

Dal primo teorema di De Morgan:  

$\overline{A + B} = \overline{A} \cdot \overline{B} \implies \overline{\overline{A + B}} = \overline{\overline{A} \cdot \overline{B}} = A + B$  

Se $\overline{\overline{A} \cdot \overline{B}} = A + B$ allora possiamo costruire una porta **OR** utilizzando due porte **NAND**.  

![universal_nand_or](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/29c80c82-2a0e-4c44-af27-7118285cb396)  

## Porta AND  

Dal secondo teorema di De Morgan:  

$\overline{A \cdot B} = \overline{A} + \overline{B} \implies \overline{\overline{A \cdot B}} = \overline{\overline{A} + \overline{B}} = A \cdot B$  

Se $\overline{\overline{A \cdot B}} = A \cdot B$ allora possiamo costruire una porta **AND** utilizzando due porte **NAND**.  

![universal_nand_and](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/cee825b3-1303-4a0e-92e2-b3adaf0b82ee)  
