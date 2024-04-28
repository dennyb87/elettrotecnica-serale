# ADC didattico  

![1bit_adc](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/1026dbda-4970-49ab-96b6-22c2a658c738)  

Didattico perche' essendo un convertitore analogico-digitale a 1 bit e' essenzialmente un comparatore con una soglia che si trova a meta' tra $0$ e il fondo scala $V_{Fs}$  

![1bit_adc_range](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/dcb47518-8c8c-4223-9871-dc23987e122c)  

Il fondo scala e' standardizzato $V_{Fs} = 10\ V$ per cui con $n = 1$ bits si ha che il convertitore presentera' in uscita $N = 2^n = 2^1 = 2$ valori. In particolare il convertitore sara' sensibile ad una specifica variazione di tensione.  

$Q = \dfrac{V_{Fs}}{N} = \dfrac{10}{2} = 5\ V$  

Il dispositivo converte allora un infinito numero di valori di tensione in ingresso in $N = 2$ valori in usci   ta.  

![1bit_adc_io](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/f10fc193-2a51-46ad-833f-d1271275cb0f)
