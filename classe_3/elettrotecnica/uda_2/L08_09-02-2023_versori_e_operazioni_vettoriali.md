# Versori  

![unit_vector](https://user-images.githubusercontent.com/7195133/217952745-789e717b-729f-4b32-b270-cc904edcf342.jpg)  

I vettori unitari (o versori) sono vettori la cui lunghezza (o modulo) e' uguale all'unita'. Dato un vettore:  

$$
\vec{a} = \begin{bmatrix}
    1 \\
    2 \\
\end{bmatrix}
$$

Si noti che e' sempre possibile rappresentarlo utilizzanto due vettori unitari opportunamente scalati. Vediamo ora in dettaglio le operazioni vettoriali che ci permettono di arrivare a tale conclusione.  

# Prodotto tra scalari e vettori    

![scaling_vectors](https://user-images.githubusercontent.com/7195133/218221904-0c656b59-946e-4863-acea-d36e0d293f36.gif)

Uno **scalare** e' semplicemente un numero, una grandezza composta dalla sola parte numerica, al contrario di un vettore che ha modulo, direzione, e verso. Si dice *"scalare"* perche' il prodotto di un vettore per uno scalare puo' aumentare o diminuire il modulo del vettore, fungendo appunto da fattore di scala.  

$$
2 \cdot \vec{v} =
2 \cdot \begin{bmatrix}
    1 \\
    2 \\
\end{bmatrix} = 
\begin{bmatrix}
    2 \\
    4 \\
\end{bmatrix}
$$  

L'operazione consiste semplicemente nel moltiplicare lo scalare per ogni componente del vettore. Dato un vettore $\vec{v}$ ed uno scalare $k$ allora si ha che il loro prodotto e':

$k\vec{v} = k(v_1, v_2, ..., v_n) = (kv_1, kv_2, ..., kv_n)$  


# Somma vettoriale 

![vector_sum](https://user-images.githubusercontent.com/7195133/218249618-3ad12f45-70d3-45ab-b319-3be990cd76b8.jpg)  

Vediamo ora la rappresentazione di $\vec{a}$ attraverso vettori unitari opportunamente scalati. 

$\vec{a} = 1 \cdot \vec{i_x} + 2 \cdot \vec{i_y}$  

Abbiamo appena definito come eseguire il prodotto tra uno scalare ed un vettore, e sappiamo che il risultato e' un vettore scalato, questo implica che $\vec{i_x} + 2\vec{i_y}$ sia una somma vettoriale. Bisogna notare che le coordinate dei vettori unitari individuano la punta di $\vec{a}$ questo diventa ancor piu' evidende spostando i vettori unitari in modo che uno parta dalla punta dell'altro.  

La somma vettoriale viene quindi definita come la somma delle componenti dei due vettori, in quanto individuano il vettore risultante, che nel nostro caso e' $\vec{a}$  

Dati due vettori $\vec{a} = (a_1, a_2, ..., a_n)\ \ \ \vec{b} = (b_1, b_2, ..., b_n)$ si ha che:  

$\vec{a} + \vec{b} = (a_1 + b_1, a_2 + b_2, ..., a_n + b_n)$  

Calcoliamo infine $\vec{a}$ partendo dai vettori unitari.  

$$
\vec{i_x} =  \begin{bmatrix}
    1 \\
    0 \\
\end{bmatrix}
$$

$$
\vec{i_y} =  \begin{bmatrix}
    0 \\
    1 \\
\end{bmatrix}
$$

$$
\vec{a} = 1 \cdot \vec{i_x} + 2 \cdot \vec{i_y} = 
\begin{bmatrix}
    1 \cdot 1 \\
    1 \cdot 0 \\
\end{bmatrix} + 
\begin{bmatrix}
    2 \cdot 0 \\
    2 \cdot 1 \\
\end{bmatrix} = 
\begin{bmatrix}
    1 \\
    0 \\
\end{bmatrix} + 
\begin{bmatrix}
    0 \\
    2 \\
\end{bmatrix} = 
\begin{bmatrix}
    1 + 0 \\
    0 + 2 \\
\end{bmatrix} =
\begin{bmatrix}
    1 \\
    2 \\
\end{bmatrix}
$$  