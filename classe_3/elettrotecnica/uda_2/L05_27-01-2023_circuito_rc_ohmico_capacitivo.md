# Circuito RC ohmico-capacitivo  

Prendiamo in considerazione un nuovo tipo circuito in cui sono presenti resistenze e condensatori. In particolare si consideri cosa accade nel circuito dopo un tempo $t$ quando i condensatori sono completamente carichi.  

![circuito_rc_ohmico_capacitivo_01](https://user-images.githubusercontent.com/7195133/215334250-39e3c629-368c-4184-9463-82b8be52f510.jpg)

Bisogna rendersi conto che se i condensatori sono carichi non puo' esserci corrente sui conduttori che interessano i condensatori, ovvero $I_A = I_B = 0$  

Sappiamo che la corrente e' un flusso di cariche $i = \dfrac{\Delta q}{\Delta t}$  

> Si utilizzano lettere minuscole per indicare che le grandezze dipendono dal tempo  

Allora possiamo osservare che $i = \dfrac{\Delta q}{\Delta t} = \dfrac{q_2 - q_1}{t_2 - t_1}$  
ma $q$ e' uguale a $C \cdot v$ e allora...  

$i = \dfrac{q_2 - q_1}{t_2 - t_1} = \dfrac{C \cdot v_2 - C \cdot v_1}{t_2 - t_1} = C \cdot \dfrac{v_2 - v_1}{t_2 - t_1}$  

Ovvero $i = C \cdot \dfrac{\Delta v}{\Delta t}$  

Si nota immediatamente che la corrente in un condensatore dipende dalla variazione di tensione nel tempo, ma se il condensatore e' carico, non c'e' variazione di tensione, o di cariche allora $i = C \cdot \dfrac{\Delta v}{\Delta t} = C \cdot \dfrac{0}{\Delta t} = 0$  


## Risolvere il circuito  

Se la corrente sui condensatori e' zero allora possiamo risolvere il circuito ignorando i condensatori.  

![circuito_ohmico_capacitivo_equivalente_01](https://user-images.githubusercontent.com/7195133/215336453-eda83654-0330-40e3-948c-4690158f6cf6.jpg)  

Le resistenze sono in serie quindi $R_{tot} = R_1 + R_2 + R_3 = 100\ \Omega$ mentre $I = \dfrac{E}{R_{tot}} = \dfrac{300}{100} = 3\ A$  

$V_1 = R_1 \cdot I = 40 \cdot 3 = 120\ V$  
$P_1 = V_1 \cdot I = 120 \cdot 3 = 360\ W$  

$V_2 = R_2 \cdot I = 50 \cdot 3 = 150\ V$  
$P_2 = V_2 \cdot I = 150 \cdot 3 = 450\ W$  

$V_3 = R_3 \cdot I = 10 \cdot 3 = 30\ V$  
$P_3 = V_3 \cdot I = 30 \cdot 3 = 90\ W$  

$P_E = E \cdot I = 300 \cdot 3 = 900\ W$  
$P_E = P_1 + P_2 + P_3 = 360 + 450 + 90 = 900\ W\ verificato\ \checkmark$  

## Carica ed energia  

Calcoliamo ora la carica e l'energia immagazzinata nei condensatori.  

$Q_A = C_A \cdot V_2 = 8 \cdot 10^{-6} \cdot 150 = 1200 \cdot 10^{-6}\ C = 1200\ \mu C = 1.2\ mC$  

$E_{NA} = \frac{1}{2} Q_AV_2 = \frac{1}{2} C_A V_2^2 = \frac{1}{2} \cdot 8 \cdot 10^{-6} \cdot 150^2 = 4 \cdot 22500 \cdot 10^{-6} = 9000 \cdot 10^{-6} = 9 \cdot 10^4 \cdot 10^{-6} = 90\ mJ$  

$Q_B = C_B \cdot V_2 =2 \cdot 10^{-6} \cdot 150 = 300 \cdot 10^{-6} = 300\ \mu C = 0.3\ mC$  

$E_{NB} = \frac{1}{2}Q_BV_2 = \frac{1}{2}C_BV_2^2 =\frac{1}{2} \cdot 2 \cdot 10^{-6} \cdot 150^2 = 22500 \cdot 10^{-6} = 22.5\ mJ$  

## Verifica su capacita' equivalente  

Possiamo verificare i calcoli comparandoli con i risultati ottenuti dalla capacita' equivalente in parallelo.  

$C_P = C_A + C_B = 8 + 2 = 10\ \mu F$

$Q_P = C_P \cdot V_2 = 10 \cdot 10^{-6} \cdot 150 = 1500 \cdot 10^{-6} = 1.5\ mJ$  

$E_{NP} = \frac{1}{2}Q_BV_2 = \frac{1}{2}C_PV_2^2 = \frac{1}{2} \cdot 10 \cdot 10^{-6} \cdot 150^2 = 112500 \cdot 10^{-6} = 112.5\ mJ$  

#
|       | $C_A$     | $C_B$      | $C_P$       |
| ----- | --------- | ---------- | ----------- |
| $Q$   | $1.2\ mC$ | $0.3\ mC$  | $1.5\ mC$   |
| $V$   | $150\ V$  | $150\ V$   | $150\ V$    |
| $E_N$ | $90\ mJ$  | $22.5\ mJ$ | $112.5\ mJ$ |
