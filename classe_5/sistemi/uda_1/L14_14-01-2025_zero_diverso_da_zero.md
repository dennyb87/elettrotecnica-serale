# Sistema con zero diverso da zero  

Questo e' un sistema dove la funzione di trasferimento nella forma $\dfrac{N(s)}{D(s)}$ ha il numeratore che si annulla con un valore di $s$ diverso da zero.  

$G(s) = 1+\dfrac{s}{10} \implies \text{zero} = -10$  

$G(j\omega) = 1+\dfrac{j\omega}{10} \implies |G| = \sqrt{1 + \bigg(\dfrac{\omega}{10}\bigg)^2}$  

Esaminiamo cosa succede al modulo di $G$ per valori estremi, ovvero quando $\omega \to 0^+$ e quando $\omega \to +\infty$ e infine quando $\omega = 10$  

$\displaystyle{\lim_{x\to 0^+}} |G| = \sqrt{1+0} = 1$  

$\displaystyle{\lim_{x\to +\infty}} |G| = \sqrt{\bigg(\dfrac{\omega}{10}\bigg)^2\cdot \bigg(\dfrac{10^2}{\omega^2}+1\bigg)} = \dfrac{\omega}{10}\cdot\sqrt{0+1} = 1 + \dfrac{\omega}{10}$  

$|G(10)| = \sqrt{1 + \bigg(\dfrac{10}{10}\bigg)^2} = \sqrt{2}$  

Per farci un'idea del comportamento della funzione nel diagramma di Bode valutiamo $|G|_{dB}$ per i valori finiti che abbiamo trovato...  

$|G|_{dB} = 20\log 1 = 0\ dB$  

$|G|_{dB} = 20\log \sqrt{2} \simeq 3\ dB$  

Mentre per valori $\gt\gt 1$ si ha $|G|_{dB} = 20\log \bigg(1+\dfrac{\omega}{10}\bigg)$  

![zero_not_zero_gsys](https://github.com/user-attachments/assets/6dab6c0b-3581-49c3-af99-1c71e0b5754a)  

