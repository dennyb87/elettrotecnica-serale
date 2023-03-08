# Calcolo induzione magnetica  

![magnetic_induction_between_wires](https://user-images.githubusercontent.com/7195133/223566586-f85545a5-cfe4-49f8-87ae-7e9498c7a9ca.jpg)

Si supponga di voler calcolare l'induzione magnetica in un punto $P$ tra i conduttori di $I_1$ ed $I_2$ sapendo che la distanza $h$ tra questi e' di $6\ m$ e che il punto $P$ dista $2\ m$ dal conduttore di $I_1$. Sappiamo anche che $I_1 = I_2 = 10\ A$ e che i conduttori sono nel vuoto.  

Calcoliamo prima di tutto $H_1$ ovvero la forza magnetizzante al punto $P$ causata dal conduttore di $I_1$ ricordando che la distanza $r$ tra $P$ e il conduttore e' $2\ m$.  

$H_1 = \dfrac{I}{2\pi r} = \dfrac{10}{2\pi \cdot 2} \simeq 0.8\ A/m$  

Troviamo ora $B_1$ ricordandoci che siamo nel vuoto.  

$B_1 = \mu_0 \cdot H_1 = 4\pi \cdot 10^{-7} \cdot 0.8 \simeq 1.005\  \mu T$  

Troviamo adesso invece $H_2$ ovvero la forza magnetizzante al punto $P$ causata dal conduttore di $I_2$ notando pero' che se $P$ e' tra i due conduttori e dista $2\ m$ dal conduttore di $I_1$ allora la distanza dal conduttore di $I_2$ sara' $h - 2 = 6 - 2 = 4\ m$. Notiamo allora che $4\ m$ e' il doppio di $2\ m$ percio':  

$H_2 = \dfrac{H_1}{2} = \dfrac{10}{2\pi \cdot 2} \cdot \dfrac{1}{2} = \dfrac{0.8}{2} \simeq 0.4\ A/m$  

$B_2 = \dfrac{B_1}{2} = \dfrac{1.005}{2} \simeq 0.5025\ \mu T$  


Per trovare infine la forza magnetizzante totale $H_{tot}$ ed il campo di induzione magnetica totale $B_{tot}$ al punto $P$ basta sommare le grandezze facendo attenzione alla direzione ed il verso dei vettori. In questo caso al punto $P$ i campi prodotti dal conduttore di $I_1$ hanno direzione uguale ma verso opposto ai campi prodotti dal conduttore di $I_2$ percio' la somma vettoriale risulterebbe in una equivalente sottrazione, ovvero:  

$H_{tot} = H_1 - H_2 = 0.8 - 0.4 = 0.4\ A/m$  

$B_{tot} = B_1 = B_2 = 1.005 - 0.5025 = 0.5025\ \mu T$  
