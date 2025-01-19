# Motore asincrono trifase  

![stator_windings](https://github.com/user-attachments/assets/7360fb5c-5f69-4c85-b91a-a03692e7ce8e)

Nel motore asincrono trifase si ha uno statore sul quale sono posti gli avvolgimenti delle tre fasi opportunamente isolate tra loro. Queste sono percorse da correnti sfasate di $120^\circ$ gradi in modo da produrre un campo magnetico rotante, o **campo induttore**.  

![rotating_magnetic_field](https://github.com/user-attachments/assets/797212e4-2ffa-410e-8ec8-dd200261b95a)  

All'interno dello statore viene posto il rotore, spesso a gabbia di scoiattolo, il quale viene cortocircuitato per formare un circuito chiuso.  

![rotori](https://github.com/user-attachments/assets/bc0b30a3-a5db-4bed-9e86-8b95fbc2606d)  

La variazione del campo induttore induce quindi una corrente nel circuito del rotore che a sua volta produce un campo magnetico detto **campo indotto**. Il campo induttore esercita allora una forza sul campo indotto e viceversa, e il rotore non avendo vincoli viene quindi messo in moto.  

![rotating_motor](https://github.com/user-attachments/assets/7a84df5b-8007-4d8c-8a2e-660a556ea1d7)  

## Velocita' angolare  

$\omega = \dfrac{\Delta \theta}{\Delta t}\ [\frac{rad}{s}]$  

Nel caso di moto circolare uniforme e' uguale a...  

$\omega = \dfrac{\Delta \theta}{\Delta t} = \dfrac{2\pi}{T} = 2\pi f$  

La velocita' angolare indica quindi la velocita' di rotazione di un certo oggetto espressa in radianti al secondo.  

## Accelerazione angolare  

$\alpha = \dfrac{\Delta \omega}{\Delta t}\ [\frac{rad}{s^2}]$  

Questa indica la variazione di velocita' dell'oggetto in rotazione espressa in radianti al secondo quadro.  

## Velocita' tangenziale (o periferica)  

$v = \omega r = 2\pi fr = \dfrac{2\pi r}{T}\ [\frac{m}{s}]$  

Questa rappresenta la velocita' di un punto posto sulla periferia del corpo in rotazione ed e' espressa in metri al secondo (essendo il radiante un numero puro). E' importante notare la dipendenza dal raggio $r$ per cui a parita' di velocita' angolare $w$ si avranno velocita' diverse in dipendenza dalla distanza dal centro. Al centro del corpo in rotatione si ha quindi velocita' tangenziale zero.  

## Giri al minuto  

$n = \dfrac{60\omega}{2\pi} = \dfrac{60\cdot \cancel{2\pi}\cdot f}{\cancel{2\pi}} = 60f\ [\text{rpm}]$  

Se la frequenza rappresenta in il numero di *"giri"* al secondo, allora l'rpm rappresenta il numero di giri al minuto. Non fa parte del sistema internazionale e' per semplicita' utilizzo $[\text{rpm}]$ come unita' di misura.  

## Momento di inerzia  

$J =  m \cdot b^2\ [kg \cdot m^2]$  

Il momento di inerzia gioca un ruolo simile alla massa nei moti lineari. Questo esprime la *resistenza* di una massa $m$ distante $b$ dall'asse di rotazione ad essere messa in moto rotatorio. La sua unita' di misura e' il kilogrammo metro quadro.  

## Moto rotatorio  

![coppia_motrice](https://github.com/user-attachments/assets/dfb952cc-ee36-4286-9639-c1a51c4c7d66)  

Applicando una coppia di forze $C = Fb$ ad un corpo si ottiene un moto rotatorio. Considerato un cilindro su cui agisce una **coppia motrice** $C_m$ questo comincera' a ruotare solo una volta vinta la **coppia resistente** $C_r$ (il carico) e la **coppia di inerzia** $J\varepsilon = J\dfrac{\Delta \omega}{\Delta t}$ (*momento fittizio che si oppone alla realizzazione del moto*) per cui la condizione  di equilibrio si esprime con:  

$C_m = C_r + J\varepsilon$  

Dove $J$ e' il momento di inerzia e dipende dalla massa e dalla geometria del corpo, per un cilindro di raggio $r$ e massa $M$ uniformemente distribuita si ha che:  

$J = \dfrac{1}{2}mr^2$  

Ne segue che con $\varepsilon = 0$ (accelerazione angolare zero) il corpo ruota a velocita' costante (oppure e' fermo), e si ha quindi l'equilibrio delle coppie $C_m = C_r$  
Con $\varepsilon \gt 0$ si ha invece $C_m \gt C_r$ dove $C_m - C_r$ rappresenta la **coppia accelerante**. Mentre con $\varepsilon \lt 0$ si ha $C_m \gt C_r$ ovvero la **coppia decelerante**.  
