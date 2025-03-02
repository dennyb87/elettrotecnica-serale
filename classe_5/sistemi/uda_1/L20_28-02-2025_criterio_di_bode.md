# Criterio di Bode  

Il criterio di stabilita' di Bode ci dice che un sistema ad anello aperto e' stabile se lo sfasamento calcolato alla pulsazione di taglio e' minore di $180^\circ$. Se la condizione e' soddisfatta allora e' stabile anche per lo stesso sistema collegato ad anello chiuso.  

```mermaid
flowchart LR
    START[ ]--"x(s)"-->node
    node(("#45;"))-->f1["F<sub>1</sub>(s)"]
    f1-->out((" "))
    out--"y(s)"-->STOP[ ]
    out-->f2["F<sub>2</sub>(s)"]
    f2-->node

    style START width:0px,height:0px;
    style STOP  width:0px,height:0px;
```

Dato il sistema ad anello chiuso si vuole verificarne la stabilita' considerato che:  

$F_1(s) = \dfrac{1}{1+\dfrac{s}{10}}$  

$F_2(s) = 10$  

Essendo in retroazione negativa...  

$G(s) = \dfrac{F_1(s)}{1+F_1(s)\cdot F_2(s)} = \dfrac{\dfrac{1}{1+\dfrac{s}{10}}}{1+\dfrac{1}{1+\dfrac{s}{10}}\cdot 10} = \dfrac{10}{s+110}$  

Il polo e' negativo $s_p = -110$ percio' il sistema e' stabile. Vogliamo ora applicare il *criterio di Bode*, quindi ricaviamo i diagrammi di Bode per lo stesso sistema, ma questa volta collegato ad **anello aperto**.  

```mermaid
flowchart LR
    START[ ]--"x(s)"-->f1["F<sub>1</sub>(s)"]
    f1-->f2["F<sub>2</sub>(s)"]
    f2--"y(s)"-->STOP[ ]

    style START width:0px,height:0px;
    style STOP  width:0px,height:0px;
```

Con il sistema ad anello aperto si ha che...  

$G(s) = F_1(s)\cdot F_2(s) = \dfrac{1}{1+\dfrac{s}{10}}\cdot 10$  

Ma allora sappiamo anche che...  

$|G|_{db} = |F_1|_{db}+|F_2|_{db}$  

Dove gli andamenti di $|F_1|_{db}$ ed $|F_2|_{db}$ sono ormai noti.  

![bode_criterion_g](https://github.com/user-attachments/assets/e493fb12-5aa2-4cc7-b55b-838b450dd1a9)  

Ricaviamo quindi il grafico della fase di $G$ ricordando che nel prodotto di numeri complessi la fase e' data da...  

$\angle G = \angle F_1 + \angle F_2$  

Dove l'andamento di $\angle F_1$ e' ormai noto, cosi' come $\angle F_2 = 0^\circ$  

![bode_criterion_phase](https://github.com/user-attachments/assets/8440c0f9-86c5-4ed7-aeda-66edae469e81)  

Il criterio di stabilita' di Bode ci dice allora che il sistema e' stabile, in quanto lo sfasamento tra ingresso ed uscita alla pulsazione di taglio e' minore di $180^\circ$ confermando il risultato ottenuto nel sistema collegato ad anello chiuso.  
