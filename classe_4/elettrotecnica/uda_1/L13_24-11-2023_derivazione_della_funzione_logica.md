# Derivazione della funzione logica  

![gates_exercise_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/00018c15-c23e-4328-ad84-d86fcc969740)  

Dato il circuito in figura si vuole trovare la funzione semplificata.  

$E = B+C$  
$F = BC$  
$G = EF = (B+C)\cdot BC$  
$D = AB$  

$Y = D+G = AB + G = AB + (B+C)\cdot BC$  
$Y = AB + BCC + BBC = AB + BC + BC$  
$Y = BC + AB = B \cdot (A + C)$  

| A   | B   | C   | A+C | Y   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   | 0   |
| 0   | 1   | 0   | 0   | 0   |
| 0   | 1   | 1   | 1   | 1   |
| 1   | 0   | 0   | 1   | 0   |
| 1   | 0   | 1   | 1   | 0   |
| 1   | 1   | 0   | 1   | 1   |
| 1   | 1   | 1   | 1   | 1   |
