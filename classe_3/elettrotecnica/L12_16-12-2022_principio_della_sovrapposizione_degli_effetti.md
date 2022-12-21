# Principio della sovrapposizione degli effetti  

In generale il principio ci dice che in un sistema lineare l'effetto complessivo  
e' uguale alla somma degli effetti individuali.  

In un circuito elettrico per effetto si intende una corrente, in quanto la corrente  
e' un effetto causato dalla tensione.  

$V = causa$  
$I = effetto$  

Questo intuisce anche dalla legge di Ohm.  
Una tensione su una resistenza produce una corrente.  

$\dfrac{V}{R} = I$  

Il principio della sovrapposizione degli effetti ci dice allora che in un circuito  
la corrente complessiva su un ramo e' la somma delle correnti prodotte dalle  
singole tensioni.

Se prendiamo allora in considerazione il seguente circuito.  

![pse_01](https://user-images.githubusercontent.com/7195133/208917689-e7577f03-3f90-4c2f-9604-41e31363e6db.jpg)  

Per trovare $I_3$ allora ci bastera' calcolare prima $I_{3A}$ ovvero l'effetto causato dal  
solo generatore $E_A$ e sommarlo all'effetto causato dal solo generatore $E_B$ ovvero

$I_3 = I_{3A} + I_{3B}$  

# Calcolo degli effetti di $E_A$  

Per calcolare i soli effetti di $E_A$ dobbiamo allora rimuovere $E_B$ dal circuito  
oppure considerarlo a tensione zero e resistenza zero.  

![pse_02](https://user-images.githubusercontent.com/7195133/208918784-0e760414-560e-4e2f-ae9a-50053a2bc92d.jpg)  

Calcoliamo quindi le resistenze in parallelo e poi la resistenza totale.  

$R_p = \dfrac{R_2 \cdot R_3}{R_2 + R_3} = \dfrac{20 \cdot 30}{20 + 30} = 12 \Omega$  

$R_{tot} = R_1 + R_p = 10 + 12 = 22 \Omega$  

Troviamo adesso le correnti.  

$I_{1A} = \dfrac{E_A}{R_{tot}} = \dfrac{100}{22} = 4.54A$  

$I_{3A} = I_{1A} \cdot \dfrac{R_2}{R_2 + R_3} = \dfrac{20}{50} = 1.816A$  

Si ha quindi che l'effetto causato dal solo generatore $E_A$ ovvero $I_{3A}$ e' uguale a $1.816A$  


# Calcolo degli effetti di $E_B$  

Stesso procedimento ma stavolta viene rimosso $E_A$  

![pse_03](https://user-images.githubusercontent.com/7195133/208972367-2cdf68ea-5196-4aec-8618-f30649323f65.jpg)  

Calcoliamo di nuovo le resistenze in parallelo e poi la resistenza totale.  

$R_p = \dfrac{R_1 \cdot R_3}{R_1 + R_3} = \dfrac{10 \cdot 30}{10 + 30} = \dfrac{300}{40} = 7.5 \Omega$  

$R_{tot} = R_2 + R_p = 20 + 7.5 = 27.5\Omega$  

$I_{2B} = \dfrac{E_B}{R_{tot}} = \dfrac{50}{27.5} = 1.818A$  

$I_{3B} = I_{2B} \cdot \dfrac{R_1}{R_1 + R_3} = 1.818 \cdot \dfrac{10}{10 + 30} = 1.818 \cdot \dfrac{1}{4} = 0.454A$  

 
# Somma degli effetti  

Una volta trovati i singoli effetti, nel nostro caso le correnti $I_{3A},\ I_{3B}$  
non dobbiamo fare altro che sommarli per trovare l'effetto complessivo.  

$I_3 = I_{3A} + I_{3B} = 1.816 + 0.454 = 2.27A$  
