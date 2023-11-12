# Porta NAND  

![nand_gate](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/4aadb056-8711-41cc-a3c4-85ac1fd66a79)  

| $A$ | $B$ | $A \cdot B$ | $\overline{A \cdot B}$ |
| --- | --- | ----------- | ---------------------- |
| 0   | 0   | 0           | 1                      |
| 0   | 1   | 0           | 1                      |
| 1   | 0   | 0           | 1                      |
| 1   | 1   | 1           | 0                      |

La porta **NAND** come si intuisce in figura e dalla tabella e' la negazione della porta **AND**. Allora entrambe le porte ci indicano quando gli ingressi sono 1-1. E' importante rendersi conto che la conoscenza dell'output non implica la conoscenza degli input, questi ultimi infatti possono essere derivati solo in specifici casi.  

$y = 0 \implies a = b = 1$  

# Porta NOR  

![nor_gate](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/132ded10-4043-4d38-bc67-5ca2b59bb491)  

| $A$ | $B$ | $A + B$ | $\overline{A + B}$ |
| --- | --- | ------- | ------------------ |
| 0   | 0   | 0       | 1                  |
| 0   | 1   | 1       | 0                  |
| 1   | 0   | 1       | 0                  |
| 1   | 1   | 1       | 0                  |

Analogamente la porta **NOR** e' la negazione della porta **OR**. Entrambe le porte ci indicano quando gli ingressi sono 0-0, negli altri casi non e' possible derivare gli input con la sola conoscenza dell'output.  

$y = 1 \implies a = b = 0$  

# Porta XOR  

![xor_gate](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1f605008-dd73-4186-87b9-f4a7e9fb5265)  

| $A$ | $B$ | $A \oplus B$ |
| --- | --- | ------------ |
| 0   | 0   | 0            |
| 0   | 1   | 1            |
| 1   | 0   | 1            |
| 1   | 1   | 0            |

La porta **XOR** (exclusive OR) ci indica allora che:  

$y = 0 \implies a = b$  
$y = 1 \implies a \ne b$  
