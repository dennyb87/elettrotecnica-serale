# Infiniti, infinitesimi ed ordini di infinito  

Si dice che una funzione $f(x)$ e' **infinita** per $x\to x_0$ se il limite tende a $\pm\infty$ mentre si dice che e' **infinitesima** per $x\to x_0$ se il limite tende a zero.  

![functions_to_infinity](https://github.com/user-attachments/assets/efb58f9c-ae30-4f6f-b6ac-1af8d2763c4b)  

E' possibile notare che, sebbene tutte le funzioni in figura siano **infinite**, alcune tendono ad infinito piu' velocemente di altre. La funzione esponenziale ad esempio e' la piu' veloce di tutte. Si parla allora di **ordini di infinito** per descrivere la velocita' con cui le funzioni tendono all'infinito. Conoscere gli ordini di infinito delle funzioni elementari ci permette ad esempio di poter risolvere forme indetereminate senza troppi sforzi.  

$\displaystyle{\lim_{x\to +\infty}}\ \frac{2^x}{x^3}$  

Sapendo che $2^x$ tende all'infinito piu' velocemente, possiamo allora dedurre che al crescere di $x$ otterremo valori di $2^x$ molto piu' grandi rispetto ad $x^3$ percio' e' possibile trattare $x^3$ come un numero finito $\ell$ e allora...  

$\displaystyle{\lim_{x\to +\infty}}\ \frac{2^x}{x^3} = \dfrac{2^x}{\ell} = \dfrac{+\infty}{\ell} = +\infty$  

Per la stessa logica invertendo la frazione si ha invece che $f(x)$ tende a zero.  

$\displaystyle{\lim_{x\to +\infty}}\ \frac{x^3}{2^x} = \dfrac{\ell}{2^x} = \dfrac{\ell}{+\infty} = 0$  

In generale se...  

$\displaystyle{\lim_{x\to x_0}}\ \dfrac{f(x)}{g(x)} = \pm\infty$  

Allora $f(x)$ e' un infinito di **ordine superiore** rispetto a $g(x)$  
Se invece...  

$\displaystyle{\lim_{x\to x_0}}\ \dfrac{f(x)}{g(x)} = 0$  

Allora $f(x)$ e' un infinito di **ordine inferiore** rispetto a $g(x)$  
Infine se...  

$\displaystyle{\lim_{x\to x_0}}\ \dfrac{f(x)}{g(x)} = \ell \ne 0$  

Allora $f(x)$ e $g(x)$ sono infiniti dello **stesso ordine** e.g.    

$\displaystyle{\lim_{x\to +\infty}}\ \dfrac{3x+2}{x-1}=\dfrac{\cancel{x}(3+\frac{2}{x})}{\cancel{x}(1-\frac{1}{x})}= 3$  
