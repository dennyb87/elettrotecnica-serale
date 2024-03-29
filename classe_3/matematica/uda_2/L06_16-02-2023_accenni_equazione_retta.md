# Accenni sull'equazione di una retta  

![straight_line_equation](https://user-images.githubusercontent.com/7195133/219866558-5bcd9881-d4b7-47f2-91eb-df7d29d4f414.jpg)  

La retta e' l'insieme di tutti i punti che vi appartengono identificabili in uno spazio bidimensionale dall'equazione:  

$y = mx + q$  

Dati $m$ e $q$ si possono sostituire ad $x$ dei valori reali per trovare i punti appartenenti alla retta. Si intuisce che questa forma ci dice che $y$ e' una funzione di $x$ ovvero:  

$y = f(x)$  

Un altro modo per scrivere l'equazione di una retta del tutto equivalente e':    

$ax + by + c = 0 \implies y = -\dfrac{a}{b}x -\dfrac{c}{b}$  


## Coefficiente angolare e intercetta verticale  

![straight_line_equation](https://user-images.githubusercontent.com/7195133/219866439-c8cedbd3-c1b5-4ab1-a1b0-59d6e7e4de22.jpg)  

Nella forma $y = mx + b$ idendtifichiamo $b$ come la quota all'origine ovvero l'intercetta verticale, quel punto della retta che interseca l'asse delle ordinate.  

Identifichiamo invece $m$ come il coefficiente angolare in quanto determina l'angolo e quindi la pendenza della retta, ovvero il rapporto incrementale, che sappiamo essere costante in una retta. Per le equazioni nella forma $y = mx + b$ questo e' dimostrabile semplicemente calcolando il rapporto incrementale tra due punti $P_A(x_0, y_0)\ P_B(x_1, y_1)$  

$y_0 = mx_0 + b$  
$y_1 = mx_1 + b$  

$\dfrac{\Delta y}{\Delta x} = \dfrac{y_1 - y_0}{x_1 - x_0} = \dfrac{(mx_1 + b) - (mx_0 + b)}{x_1 - x_0} = \dfrac{mx_1\ \cancel{+ b} - mx_0\ \cancel{- b}}{x_1 - x_0} = \dfrac{m \cdot \cancel{(x_1 - x_0)}}{\cancel{x_1 - x_0}} = m$  

Diventa evidente che $m$ e' costante e che rappresenta il rapporto con cui $y$ varia al variare di $x$. Possiamo adesso identificare immediatamente due rette parallele in quanto avranno lo stesso coefficiente angolare ma intercetta diversa. Diventa facile anche intuire la loro pendenza grazie al segno del coefficiente angolare.  

![parallel_lines](https://user-images.githubusercontent.com/7195133/219866868-9d603a61-bd5a-4c0c-8fd3-c8f6ddf242b1.jpg)  

Allora diventa ovvio che non esistendo un punto in cui due rette parallele si intersecano, non e' possibile trovare una soluzione al sistema delle loro equazioni. Se invece il coefficiente angolare e' diverso, allora risolvendo il sistema, quindi trovando i valori delle incognite che rendono entrambe le equazioni vere, possiamo trovare le coordinate del punto in cui le due rette si intersecano.  

$$
\begin{cases}
  \begin{aligned}
    y &= 2x + 2 \\
    y &= 3x + 2 \\
  \end{aligned}
\end{cases}
$$  

$$
\begin{cases}
  \begin{aligned}
    y &= 2x + 2 \\
    2x + 2 &= 3x + 2 \\
  \end{aligned}
\end{cases}
$$  

$$
\begin{cases}
  \begin{aligned}
    y &= 2x + 2 \\
    x &= 0 \\
  \end{aligned}
\end{cases}
$$  

$$
\begin{cases}
  \begin{aligned}
    y &= 2 \\
    x &= 0 \\
  \end{aligned}
\end{cases}
$$  

![intersezione_rette](https://user-images.githubusercontent.com/7195133/219903132-e6b3fd86-0d8f-438a-bfd4-9f8b6471d4e5.jpg)