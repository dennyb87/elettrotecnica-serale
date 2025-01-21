# Sistema a funzione di trasferimento costante  

$y = Gx$  

Questo tipo di sistema non ha ne' zeri ne' poli, ha appunto una fuzione di trasferimento costante, ad esempio:  

$|G| = 10$  

La funzione non dipende quindi da $\omega$ per cui per qualunque frequenza si avra' in uscita 10 volte il segnale in ingresso. In particolare con questo tipo di sistemi si ha:  

* $|G| \gt 1$ amplificatore
* $|G| = 1$ segnale invariato
* $|G| \lt 1$ riduttore

Vediamo il diagramma lineare.  

![linear_constant_gsys](https://github.com/user-attachments/assets/e9dff872-2efd-451b-b507-fa26427ec4ba)  

Nei diagrammi di Bode si utilizzano i decibel per rappresentare i valori sull'asse delle ordinate. Per definizione il modulo di $G$ in decibel e' uguale a:    

$|G|_{dB} = 20\log |G|$  

In questo caso...  

$|G|_{dB} = 20\log 10 = 20\ dB$  

![bode_constant_gsys](https://github.com/user-attachments/assets/e5fb891f-3234-4da0-8261-1acc023c5070)  


# Sistema con zero nell'origine  

$|G| = \omega$  

In questo caso il sistema non ha poli, ma ha uno zero nell'origine. Nel grafico lineare si ha quindi una retta che passa appunto per l'origine quando $\omega = 0$  

![linear_zero_origin_gsys](https://github.com/user-attachments/assets/b32f0458-469b-4983-92a0-87392e64668b)  

In modo analogo, nel diagramma di Bode si ha una retta con pendenza $20\ \frac{{dB}}{dec}$  

$|G|_{dB} = 20\log \omega$  

![bode_zero_origin_gsys](https://github.com/user-attachments/assets/b33b746c-74bb-47d1-9987-51b61491d114)  

Questo e' anche detto **filtro derivatore** in quanto amplifica in dipendenza della frequenza. Maggiore e' la frequenza, maggiore e' il guadagno.  
