# Impianto di terra  

![dispersore_emisferico](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/43e994e3-a702-4b19-b4c9-a85274368a40)  

Consideriamo il caso ideale di un dispersore emisferico di raggio $r_0$ che disperde una corrente $I$ in un terreno con resistivita' costante $\rho_E$.  

Per calcolare la resistenza totale dalla superficie del dispersore $r_0$ a distanza infinita $ dobbiamo allora sommare tutti i contributi di $dr$ da $r_0$ a $\infty$ dove $dr$ e' la distanza infinitesima percorsa dalla corrente.  

$R_E = \int_{r_0}^\infty \rho_E \cdot \dfrac{dr}{2\pi r^2} = \dfrac{\rho_E}{2\pi r_0}$  

Abbiamo essenzialmente utilizzato la seconda legge di Ohm per giungere alla conclusione che la resistenza di terra $R_E$ e' direttamente proporzionale alla resistivita' del terreno $\rho_E$ ed inversamente proporzionale alla distanza dal dispersore $r$.  

Diventa evidente allora che ad una certa distanza la sezione diventa tale da rendere la resistenza praticamente nulla, mentre in prossimita' del dispersore la superficie attraversata dalla corrente diminuisce e la resistenza aumenta di conseguenza. Allora va da se che e' sempre piu' conveniente cercare di ridurre la resistivita' in prossimita' del dispersore, zona in cui si concentra maggiormente la resistenza di terra, ovvero intorno intorno ad $r_0$.  

![distanza_tensione_terra](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/379b881d-b242-46b1-92f6-0c845d066b8b)  

## Tipi di dispersori  

I dispersori possono essere **intenzionali** ovvero installati appunto intenzionalmente per scopi inerenti alla messa a terra, oppure **di fatto** i quali diventano dispersori solo incidentalmente e.g. ferri di armatura, tubazioni metalliche.  
