### FAD - CLASSE 3 - SISTEMI AUTOMATICI - UDA2
# SISTEMA ELETTRICO ENERGIA

## Quesiti 

**1. Quali sono le fonti primarie di energia ?**  

Le fonti primarie sono: radiante (sole), fluidodinamica (vento, cadute d'acqua, maree), chimica (biomasse, combustibili fossili e.g. gas, carbone, petrolio), endogena (calore endogeno della terra), nucleare (combustibili fissili)

**2. In che modo le fonti primarie di energia possono essere convertite in energia elettrica ?**  

Dipende dalla fonte, sono possibili conversioni dirette come nel caso del fotovoltaico, tutte le altre fonti richiedono una o piu' trasformazioni e.g. termica > meccanica > elettrica, ognuna di queste fa affidamento ad una turbina che aziona un generatore.

**3. Quali sono le possibili trasformazioni di energia elettrica ?**  

L'energia elettrica puo' essere trasformata in energia termica, meccanica, luminosa, o utilizzata per il trattamento dell'informazione.   

**4. Perche' l'energia elettrica e' considerata un vettore energetico ?**  

L'energia elettrica e' un vettore (trasportatore) energetico in quanto si presta ad essere trasportata lontano dalla fonte primaria da cui e' stata generata per poi essere convertita nel luogo di utenza.  

**5. Descrivere, utilizzando uno schema a blocchi, le trasformazioni di energia in una centrale idroelettrica.**  

```mermaid
flowchart LR
    bacino_idrico--->turbina_idraulica--->generatore--->energia_elettrica
```  

**6. Descrivere, utilizzando uno schema a blocchi, le trasformazioni di energia in una centrale termoelettrica**

```mermaid
flowchart LR
    carbone--->caldaia--->turbina_a_vapore--->generatore--->energia_elettrica
```  

**7. Qual e' la struttura del sistema elettrico per l'energia ?**  

Il sistema elettrico e' composto da pochi generatori di grande taglia, e tanti piccoli utilizzatori.  

```mermaid
flowchart LR
    centrale--->trasformatore_elevatore--->linea_AT--->trasformatore_MT--->linea_MT--->cabina_trasformazione_BT--->linea_BT--->utenza
```     

**8. Che cosa si intende per produzione, trasmissione, distribuzione e utilizzazione di energia elettrica ?**  

Per produzione si intende il processo per cui l'energia viene trasformata in energia elettrica partendo da una fonte primaria. La trasmissione consiste invece nel trasferimento di grandi quantita' di energia su grandi distanze in alta e media tensione. Con distribuzione si intende il trasferimento di energia alle utenze su brevi distanze ed in bassa (in casi particolari media o alta) tensione.  

**9. Che cosa si intende per BT, MT, AT ?**  

Servono per indicare i valori di tensione, generalmente in alternata in un contesto di trasmissione e distribuzione.  

Bassa Tensione $0V \le BT \le 1000V$  
Media Tensione $1kV < MT \le 30kV$
Alta Tensione $30kV < AT$

**10. Che cosa si intende per generazione distribuita di energia elettrica ? Quali sono i vantaggi ?**  

In questo nuovo modello i consumatori, che nel sistema tradizionale consumano solo energia, possono anche avere il ruolo di produttore di energia elettrica, si dicono quindi **prosumer**, ovvero produttori e consumatori. Questo permette l'utilizzo di fonti energetiche alternative per la produzione locale, quindi un minore costo di distribuzione. La vicinanza degli impianti di produzione dell'energia ai punti di consumo finale (utenza) consente un minore trasporto dell'energia elettrica e una minore dispersione.  

**11. Che cosa e' il diagramma di carico nel sistema elettrico per l'energia ?**  

Si definisce diagramma di carico la curva della potenza attiva prelevata dall'utenza in funzione del tempo. La produzione viene stimata attraverso l'analisi di dati giorno per giorno in quanto non e' possibile fare previsioni accurate a lungo termine.  


**12. Elencare e descrivere i punti di forza e di debolezza del sistema elettrico per l'energia.**  

### Punti di forza
* flessibilita' di produzione
* elevato rendimento di trasimssione e distribuzione
* praticita' e sicurezza d'uso

### Punti di debolezza
* perdita netta nel processo di produzione
* equilibrio tra produzione e carico