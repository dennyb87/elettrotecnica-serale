# Continuita'  

Una funzione $f(x)$ si dice continua in un punto se $\displaystyle{\lim_{x\to x_0}} f(x) = f(x_0)$ ovvero il limite esiste e coincide con il valore che la funzione assume per $x_0$. Vedremo piu' avanti che una funzione composta e' continua se lo sono anche le funzioni che la compongono. Ad esempio non e' necessario studiare la continuita' di $x^2+x+c$ in quanto le sue componenti sono tutte continue.  

# Discontinuita' di prima specie  

![salto](https://github.com/user-attachments/assets/d84ad7cf-f0bf-474e-a8e3-1acf7628828e)  

$\displaystyle{\lim_{x\to x_0^-} f(x) \ne \lim_{x\to x_0^+}f(x)}$  

Questo tipo di discontinuita' si presenta come un *"salto"* nella funzione, formalmente esiste un **limite finito sinistro** e un **limite finito destro** ma questi **non coincidono**. Il valore assoluto della differenza tra questi limiti rappresenta quindi il *"salto"*...  

$\Delta y = \bigg|\displaystyle{\lim_{x\to x_0^-} f(x) - \lim_{x\to x_0^+}f(x)}\bigg|$  

# Discontinuita' di seconda specie  

![seconda_specie](https://github.com/user-attachments/assets/bfe8df6b-992a-422e-8ad0-7e0efae5309d)  

Si dice che nel punto $x_0$ la funzione ha una discontinuita' di seconda specie se almeno uno dei limiti, destro o sinitro, non esiste o e' infinito.  

# Discontinuita' di terza specie  

In questo caso si hanno invece due possibilita':  

1. il limite esiste ma $f(x_0)$ non esiste
2. $f(x_0)$ esiste ma $\displaystyle{\lim_{x\to x_0} f(x) \ne f(x_0)}$

![terza_1](https://github.com/user-attachments/assets/c7505935-241d-45d7-bb6b-ce7bd50c1e4b)  

Nel primo caso si ha un vero e proprio *"buco"* nella funzione in quanto $f(x_0)$ non esiste.  

![terza_2](https://github.com/user-attachments/assets/c8fe5503-371b-45f7-80dd-738b86de6c08)  

Nel secondo caso si ha invece una deviazione per $f(x_0)$  
