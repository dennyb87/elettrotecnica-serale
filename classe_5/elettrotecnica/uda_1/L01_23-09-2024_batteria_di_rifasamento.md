# Batteria di rifasamento  

![batteria_rifasamento](https://github.com/user-attachments/assets/25a02220-9111-483c-9a9d-1d2864c2c079)  

In un sistema trifase essendo composta da tre linee, si devono utilizzare tre condensatori in due possibili configurazioni:
* $C_\Delta$ triangolo
* $C_Y$ stella 

Nella configurazione a stella si ha che la potenza reattiva totale e' data da:  

$Q_{Ytot} = 3X_CI_C^2$  

Ovvero 3 volte la $Q_Y$ di ogni singolo condensatore. Ma per la legge di Ohm la corrente sul singolo condensatore e'...  

$I_C = \dfrac{V}{\sqrt{3}X_C}$  

Dove $V$ e' la tensione concatenata e.g. $V_{12}$ della linea. Sostituendo alla prima equazione otteniamo:  

$Q_{Ytot} = \cancel{3X_C} \dfrac{V^2}{\cancel{3}X_C^{\cancel{2}}} = \dfrac{V^2}{X_C}$  

$Q_{Ytot} = \dfrac{V^2}{X_C} \implies X_C = \dfrac{V^2}{Q_{Ytot}}$  

$X_C = \dfrac{1}{\omega C} = \dfrac{V^2}{Q_{Ytot}}$  

$C = C_Y = \dfrac{Q_{Ytot}}{\omega V^2}$  

Nel caso della configurazione a triangolo si ha che la corrente sul condensatore e' invece:  

$I_C = \dfrac{V}{X_C}$  

Non contenendo il fattore $\sqrt{3}$ si resta quindi con un fattore $3$ che non viene cancellato per cui...  

$C_\Delta = \dfrac{Q_{Ytot}}{3\omega V^2}$  

Solitamente, almeno in bassa tensione, e' preferibile  utilizzare il collegamento a triangolo, in quanto tre volte piu' piccolo di quello a stella che risulterebbe inutilmente sovradimensionato.  

$C_Y = 3C_\Delta$  
