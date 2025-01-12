# Ricerca degli asintoti  

Data un'equazione $y = \dfrac{3x}{x^2-1}$ e' possibile derivare gli asintoti verticali e orizzontali dal suo dominio, in questo caso il numeratore non da' problemi per cui esaminiamo solo il denominatore:  

$x^2 -1 \ne 0 \implies x \ne \pm 1$  

$D: (-\infty,-1)\cup(-1,+1)\cup(+1, +\infty)$  


## Asintoti verticali  

Conoscendo il dominio, e' possibile ricavare gli asintoti orizzontali valutando il limite con $x \to x_0$ per tutti gli **estremi finiti** di ogni intervallo, in questo caso $x_0 = \pm 1$  

$\displaystyle{\lim_{x\to +1^+}}\ \dfrac{3x}{x^2-1} = \dfrac{3x}{1.001-1} = \dfrac{3x}{0^+} = +\infty$  

$\displaystyle{\lim_{x\to +1^-}}\ \dfrac{3x}{x^2-1} = \dfrac{3x}{0.999-1} = \dfrac{3x}{0^-} = -\infty$  

$\displaystyle{\lim_{x\to -1^+}}\ \dfrac{3x}{x^2-1} = \dfrac{3x}{0.999-1} = \dfrac{3(-1^+)}{0^-} = +\infty$  

$\displaystyle{\lim_{x\to -1^-}}\ \dfrac{3x}{x^2-1} = \dfrac{3x}{1.001-1} = \dfrac{3(-1^-)}{0^+} = -\infty$  

In questo caso si hanno allora due **asintoti verticali bilateri**, ovvero l'asintoto si presenta sia da destra che da sinistra per le equazioni:   

$x = -1$  
$x = +1$  

## Asintoti orizzontali  

Per ricavare gli asintoti orizzontali e' sufficiente valutare il limite con $x \to x_0$ per gli **estremi infiniti** di ogni intervallo, in questo caso $x_0 = \pm\infty$  

$\displaystyle{\lim_{x\to +\infty}}\ \dfrac{3x}{x^2-1} = \dfrac{3x}{x^2(1-\frac{1}{x^2})} = \dfrac{3}{x(1-0)} = 0$  

$\displaystyle{\lim_{x\to -\infty}}\ \dfrac{3x}{x^2-1} = \displaystyle{\lim_{x\to +\infty}}\ \dfrac{3x}{x^2-1} = 0$  

In questo caso si ha allora un **asintoto orizzontale bilatero**, ovver l'asintoto si presenta sia a destra che a sinistra della retta delle ordinate per l'equazione:  

$y = 0$  

![asymptote_seeking](https://github.com/user-attachments/assets/0667f736-8fd3-4f98-aa76-e4ed9a4531ca)  
