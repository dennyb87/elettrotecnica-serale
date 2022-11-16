# Applicazioni delle leggi di Kirchhoff  

Di seguito si ripetono le gia' affrontate leggi di Kirchhoff.  

## Prima legge o legge dei nodi

La somma delle correnti entranti in un nodo e' uguale alla somma delle  
correnti uscenti.  
$I_1 = I_2 + I_3$  

![kirchhoff_1](https://user-images.githubusercontent.com/7195133/195977379-bbc3de68-a649-4520-9e59-a086dc6534dd.jpg)  

## Seconda legge o legge delle maglie

La somma algebrica di tutte le differenze di potenziale che si incontra  
in una maglia e' uguale a zero.  

Si noti come $V_s = V_{R_1} + V_{R_2} + V_{R_3}$ oppure $V_s - V_{R_1} - V_{R_2} - V_{R_3} = 0$

![kirchhoff_2](https://user-images.githubusercontent.com/7195133/195985646-8b277b29-6bf0-44a7-9a6d-08240a51b0e8.jpg)  

# Prima legge di Kirchhoff per derivare la formula delle resistenze in parallelo  

Grazie alla prima legge e' possibile derivare le correnti e le altre grandezze  
elettriche semplicemente riarrangiando i termini di equazioni note.  
Si prenda in considerazione il seguente circuito.  

![current_in_parallel_resistors](https://user-images.githubusercontent.com/7195133/202259331-f47e13bd-f296-4a7b-9324-817e9f898e57.jpg)  

Sappiamo grazie alla prima legge che $I = I_1 + I_2$  
Sappiamo anche che due o piu' resistenze in parallelo contribuiscono ad una  
singola caduta di potenziale, ovvero ai loro capi c'e' la stessa tensione.  
Da questo si deduce che $I_1 = \frac{V_b}{R_1}$ e che $I_2 = \frac{V_b}{R_2}$ e di conseguenza che $I = \frac{V_b}{R_1} + \frac{V_b}{R_2}$  

Riarrangiando i termini si ha allora che:

$I = V_b(\frac{1}{R_1} + \frac{1}{R_2})$  
$\frac{I}{V_b} = \frac{1}{R_1} + \frac{1}{R_2}$  

Trovando il reciproco $\frac{V_b}{I} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2}}$ abbiamo in effetti trovato la resistenza equivalente  
dato che $R_{eq} = \frac{V_b}{I} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2}}$  

Bisogna ora ricordarsi che $\frac{1}{a} + \frac{1}{b} = \frac{a + b}{a \cdot b}$  

Allora si ha che $R_{eq} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2}} = \frac{1}{\frac{R_1 + R_2}{R_1 \cdot R_2}} = \frac{R_1 \cdot R_2}{R_1 + R_2}$  

Abbiamo appena derivato la formula delle resistenze  in parallelo usando la  
legge di Ohm e la prima legge di Kirchhoff.