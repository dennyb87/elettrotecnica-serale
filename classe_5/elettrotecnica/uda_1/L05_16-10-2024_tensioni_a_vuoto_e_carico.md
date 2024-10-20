# Tensioni a vuoto e a carico  

![tranformer_secondary_circuit](https://github.com/user-attachments/assets/5b8688e8-05e7-4570-bef1-07eed9778d16)  

Nelle nostre applicazion i parametri trasversali possono essere ignorati, per cui per semplificare il circuito e' possibile portare i parametri longitudinali sul secondario. Questi sono detti di corto-circuito $cc$ in quanto vengono stimati grazie a un test di corto circuito.  

$R_{2cc} = R_1+R_2$  

$X_{2cc} = X_1+X_2$  

A vuoto (ovvero senza carico, indicato con il suffisso zero) la corrente sui parametri longitudinalie e' zero per cui non si ha caduta di tensione e ne segue che $V_{20} = \dfrac{N_2}{N_1}V_1$  

> transformer with load here

Aggiunto un carico si avra' una nuova tensione $V_2 < V_{20}$ che vettorialmente e' possibile rappresentare come segue.  

![transformer_real_vectors](https://github.com/user-attachments/assets/ae1003d0-380c-4df4-b77e-7d15f247b9e9)  

Assumendo un carico induttivo, la corrente $I_2$ sara' in ritardo rispetto alla nuova tensione $V_2$ di un angolo $\varphi$. La tensione $R_{2cc}I_2$ sara' invece in fase con la corrente, mentre la tensione $X_{2cc}I_2$ con reattanza assunta induttiva sara' di nuovo in anticipo rispetto a $I_2$.  

La reattanza longitudinale causa quindi un ulteriore sfasamento di un certo angolo $\epsilon$ non nullo ma che realisticamente e' molto piccolo per cui trascurabile.  

![transformer_vector_approximation](https://github.com/user-attachments/assets/f1be4f76-bc42-4876-b0ad-68b25c4c0d0d)  

In definitiva e' possibile calcolare la caduta di tensione causata dai parametri longitudinali con:  

$\Delta V = V_{20} - V_2 = I_2(R_{2cc}\cos\varphi+X_{2cc}\sin\varphi)$  
