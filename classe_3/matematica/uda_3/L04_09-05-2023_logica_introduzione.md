# Introduzione alla logica matematica   

La logica matematica nasce dall'esigenza di formalizzare il metodo scientifico per poter giungere a conclusioni ed effettuare dimostrazioni. Come nel metodo scientifico esiste una **logica induttiva** ed una **logica deduttiva**.  

La **logica induttiva** si basa sull'osservazione di un fenomeno particolare per formulare un principio generale, esempio: 

1. Ho visto un corvo ed era nero
2. Ho visto un secondo corvo ed era nero
3. Ho visto un terzo corvo ed era nero

Conclusioni:

1. Il prossimo corvo che vedro' sara' probabilmente nero
2. Tutti i corvi sono probabilmente neri

E' importante rendersi conto che in un argomento induttivo non vi e' certezza ma soltanto un grado di probabilita' maggiore di zero e minore di uno.


Nella **logica deduttiva** invece, che utilizza principi generali o fatti che non richiedono verifica, e' impossibile che la conclusione di un ragionamento sia falsa se le sue premesse sono vere, ad esempio:  

1. Tutti gli uomini sono mortali
2. Socrate e' un uomo

Conclusione:

1. Socrate e' mortale


## Proposizioni  

Una proposizione e' un'affermazione, una frase a cui si puo' attribuire un valore di verita' e.g. *"4 e' un numero pari"* e' indubbiamente una proposizione ed e' anche vera, mentre *"Giulia e' simpatica"* dato che non e' possibile stabilirlo con criterio oggettivo non puo' essere considerata una proposizione. 

Esistono preposizioni elementari (semplici o atomiche) che presentano un solo predicato verbale e.g. *"Roma **e'** la capitale d'Italia"* oppure preposizioni composte (o molecolari) che utilizzano piu' predicati verbali e.g. "se **torno** a casa ti **accompagno** alla stazione". In queste ultime vengono utilizzati anche cinque connettivi logici *"non, e, o, se ... allora, se e solo se"* appunto per legare tra loro proposizioni elementari e.g. *"**se** un numero e multiplo di 4, **allora** e' pari"*.  


## Connettivi come operazioni  

Si vedano gli esempi di negazione (*not*), congiunzione (*and*), e disgiunzione (*or*).  

|              |             |             |
| ------------ | ----------- | ----------- |
| negazione    | not $p$     | $\bar{p}$   |
| congiunzione | $p$ and $q$ | $p \land q$ |
| disgiunzione | $p$ or $q$  | $p \lor q$  |


## L'implicazione  

$p \implies q$  

Questa notazione rappresenta due preposizioni legate da il connettivo *"se ... allora"* e viene chiamata implicazione, dove $p$ e $q$ sono anche chiamate rispettivamente **premessa** e **conseguenza**.  

*"Essere milanesi implica essere italiani"*  

$p = essere\ milanesi$  
$q = essere\ italiani$  

$p \implies q$  

Si puo' esprimere anche come:

* se sei milanese allora sei italiano
* essere milanese e' condizione sufficiente per essere italiano
* essere italiano e condizione necessaria per essere milanese

Ne consegue che non essere italiani comporta non essere milanesi, ovvero:  

$\bar{q} \implies \bar{p}$