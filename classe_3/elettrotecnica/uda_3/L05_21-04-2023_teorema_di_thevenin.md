# Teorema di Thevenin  

![thevenin_rough_example](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/c373d98e-b55e-4bac-a5b7-3d0d74a8903d)  

Il teorema di Thevenin ci dice che un circuito complesso puo' essere visto come una black box composta da un generatore di tensione $E_{th}$ in serie ad una resistenza $R_{th}$ dove:

* $E_{th}$ e' la **tensione a vuoto** tra due punti scelti in modo arbitrario
* $R_{th}$ e' la **resistenza totale senza generatore**

Prendiamo in considerazione il seguente circuito.  

![thevenin_example_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/07f960da-d5ed-4f9f-a3ba-f6dbfa8d612f)  

![thevenin_example_02](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/e29f06cf-ebc7-45e8-94b9-05e4db924708)

Thevenin ci dice allora che dal punto di vista di $R_3$ e' possibile semplificare il circuito rappresentandolo  come un generatore $E_{th}$ in serie ad una resistenza $R_{th}$. Sappiamo che $E_{th}$ e' la tensione a vuoto tra due punti, in questo caso $E_{th} = V_{BC_0}$. Troviamo allora $V_{BC_0}$ grazie al partitore di tensione, ricordandoci di ignorare $R_3$.

$V_{BC_0} = E \cdot \dfrac{R_2}{R_1 + R_2} = 60 \cdot \dfrac{6}{1.5 + 6} = 48\ V$  

![thevenin_example_03](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/152de5ef-3bfd-4daa-91ed-cc2c16be6d77)  

Troviamo infine la resistenza equivalente $R_{th}$ cortocircuitando il generatore.  

$R_{th} = R_{BC} = \dfrac{R_1 \cdot R_2}{R_1 + R_2} = \dfrac{1.5 \cdot 6}{1.5 + 6} = 1.2\ \Omega$  

Si ha allora che il circuito di Thevenin equivalente e' composto da un generatore $E_{th} = 48\ V$ in serie ad una resistenza $R_{th} = 1.2\ \Omega$.  

![thevenin_example_04](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/699c4796-4e6b-49f4-afde-36cc0b02d682)  
