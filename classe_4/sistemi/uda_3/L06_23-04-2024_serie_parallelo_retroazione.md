# Ripasso collegamenti  
## Serie  

```mermaid
flowchart LR
    in(" ")--"x"-->G1
    G1--"w"-->G2
    G2--"y"-->out(" ")
```

Nel collegamento serie si ha che $w = G_1x$ per cui...  

$y = G_2w = G_2G_1x$  

La funzione di trasferimento del sistema allora sara':  

$G_{tot} = \dfrac{y}{x} = \dfrac{G_2G_1\cancel{x}}{\cancel{x}} = G_2G_1$  

## Parallelo  

```mermaid
flowchart LR
    in(" ")--"x"-->node
    node(" ")-->G1
    node-->G2
    G1-->sum("+")
    G2-->sum
    sum--"y"-->out(" ")
```

Nel collegamento parallelo la funzione di trasferimento e' invece:  

$G_{tot} = G_1+G_2$  

## Retroazione positiva  

```mermaid
flowchart LR
    in(" ")--"x"-->sum("+")
    sum-->G1
    G1-->node(" ")
    node-->G2
    node--"y"-->out(" ")
    G2--"positive"-->sum
```

In retroazione positive si ha invece che...  

$G_{tot} =\dfrac{G_1}{1 - G_1G_2}$  

## Retroazione negativa  

```mermaid
flowchart LR
    in(" ")--"x"-->sum("+")
    sum-->G1
    G1-->node(" ")
    node-->G2
    node--"y"-->out(" ")
    G2--"negative"-->sum
```

In retroazione positive si ha invece che...  

$G_{tot} =\dfrac{G_1}{1 + G_1G_2}$  

