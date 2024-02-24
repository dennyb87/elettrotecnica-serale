# Legge di Ohm generalizzata  

![capacitive_test_01](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/57d364ec-14c1-44e3-9d06-2a37aafb8028)  

Si vuole esaminare l'opposizione al passaggio di corrente in un circuito puramente capaticivo come in figura. Registrando i valori delle grandezze e' possibile calcolare il rapporto tra tensione e corrente. Mentre in un circuito puramente resistivo questo coincide con la **resistenza**, in generale prende il nome di **impedenza**, ovvero la capacita' di un circuito opporsi al passaggio di cariche.  

| $f[Hz]$ | $C[F]$ | $V[V]$ | $I[A]$ | $Z[\Omega]$ |
| ------- | ------ | ------ | ------ | ----------- |
| 0.5     | 0.1    | 10     | 3.14   | 3.185       |
| 0.5     | 0.1    | 20     | 6.28   | 3.185       |
| 0.5     | 0.1    | 30     | 9.42   | 3.185       |

La tabella ci mostra che l'impedenza resta costante evidenziando la validita' della legge di Ohm anche in un circuito puramente capacitivo.  

$Z = \dfrac{V}{I}$  

L'impedenza $Z$ pero' e' una grandezza che deve tenere conto dei diversi tipi opposizione al passagio di cariche, per cui se in un circuito puramente resistivo si parla di resistenza dove $Z = R$ in un circuito puramente capacitivo si parla di **reattanza capacitiva** $X_c$ dove $Z = X_c$  

| $f[Hz]$ | $C[F]$ | $V[V]$ | $I[A]$ | $Z[\Omega]$ |
| ------- | ------ | ------ | ------ | ----------- |
| 1       | 0.1    | 10     | 6.3    | 1.587       |
| 1       | 0.1    | 20     | 12.6   | 1.587       |
| 1       | 0.1    | 30     | 18.9   | 1.587       |

| $f[Hz]$ | $C[F]$ | $V[V]$ | $I[A]$ | $Z[\Omega]$ |
| ------- | ------ | ------ | ------ | ----------- |
| 0.5     | 0.2    | 10     | 6.28   | 1.592       |
| 0.5     | 0.2    | 20     | 12.56  | 1.592       |
| 0.5     | 0.2    | 30     | 18.84  | 1.592       |


Variando la capacita' e la frequenza si puo' osservare una variazione di corrente, cosi' come di impedenza. In particolare e' dimostrabile che la **reattanza capacitiva** puo' essere descritta come segue:  

$X_c = \dfrac{1}{\omega \cdot C}$  
