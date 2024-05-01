# Grandezze nel sistema trifase  

![grandezze_trifase](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/6639bd19-7ff7-459b-b25d-933549e6f1e3)  

Il sistema trifase puo' essere diviso in tre parti:
* generatore 
* linea
* carico

Ognuno di questi elementi contiene dei rami detti **fase**. Mentre nel generatore e nel carico si parla di tensioni e **correnti di fase**, nella parte centrale, quella di linea, si parla di **tensioni contatenate** o di linea e **correnti di linea**.  

Dato che $I_1 = I_2 = I_3$ mentre $V_{12} = V_{23} = V_{31}$ per comodita' si utilizza $V$ ed $I$ per indicare la tensione e la corrente di linea. In modo analogo avviene lo stesso con le tensioni e le correnti di fase $V_F$ e $I_F$ cosi' come le tensioni e le correnti del generatore $E$ e $I_{GF}$  


## Carico a stella  

![carico_a_stella](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/040d398d-85b9-4fec-a8a5-1dd508ee220e)  

E' importante notare che nel carico a stella mentre per le correnti possiamo dire che $I = I_F$ non e' possibile fare lo stesso con le tensioni in quanto per la seconda legge di Kirchhoff...  

$\vec{V} = \vec{V_{F1}} - \vec{V_{F2}} \implies V = \sqrt{3} \cdot E$  


## Carico a triangolo  

![carico_a_triangolo](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/b0b8e2c6-3c47-4a18-a1aa-6fc6c96443f8)  

In questo caso invece, sempre per le leggi di Kirchhoff...  

$V = V_F$  

$\vec{I} = \vec{I_{F1}} - \vec{I_{F2}} \implies \sqrt{3} \cdot I_F$  

## Carico equilibrato  

Quando i vettori delle impedenze del carico coincidono, ovvero quando hanno lo stesso modulo e fase, allora si dice che il carico e' **equilibrato**. In ogni altro caso si ha invece un carico **squilibrato**. Ad esempio, nel caso particolare di tre carichi, due resistivi ed uno induttivo, pur avendo la stessa impedenza di $10\ \Omega$ saremmo comunque di fronte ad un carico squilibrato causato da uno sfasamento vettoriale.  
