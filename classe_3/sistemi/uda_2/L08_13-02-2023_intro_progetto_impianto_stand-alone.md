# Introduzione al progetto di un impianto fotovoltaico stand-alone  

Stand-alone significa un impianto isolato (anche detto a isola), quindi non collegato alla rete (off-grid). Per progettare un impianto bisogna prima di tutto conoscere il **fabbisogno energetico**, ovvero la stima del consumo di energia richiesto dall'utente, e la quantita' di **energia disponibile** sul luogo di utenza.  

![photovoltaic-stand-alone](https://user-images.githubusercontent.com/7195133/219939328-dcd707ac-4b8a-485c-9394-84241581fb78.jpg)

Un impianto del genere e' composto da:   

* pannelli solari fotovoltaici
* regolatore di carica
* accumulatori
* iverter $DC \implies AC$

La funzione principale del **regolatore di carica** e' quella di assicurare una corrente costante ai carichi, prelevandola dai pannelli e/o dalla batteria. Si occupa inoltre di interrompere la carica quando la batteria e' completamente carica e di disconnettere i carichi quando la batteria e' scarica, evitando cosi' stati di sovraccarica o di scarica profonda della batteria, prolungando la vita della batteria. Inoltre impedisce che il pannello venga visto come un carico da parte degli accumulatori, per esempio di notte quando non c'e' produzione di energia.  

## PVGIS - Photovoltaic Geograhical Information System  

Una volta stimato il fabbisogno energetico e' possibile calcolare il tipo ed il numero di pannelli necessari per soddisfarlo nel luogo di utenza grazie a banche dati disponibili online come [PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/en/) che fornisce dati sull'irraggiamento solare a livello globale.  

![pvgis_preview](https://user-images.githubusercontent.com/7195133/219940442-a72bd097-f732-4b09-a423-4913969a3cdd.jpg)  

## Pannelli monocristallini vs policristallini  

![poly-vs-monocrystalline](https://user-images.githubusercontent.com/7195133/219941673-0b6ed450-c4db-4914-ae1e-03a9815cd0d1.jpg)  

I pannelli detti monocristallini hanno celle che sono state create da un singolo cristallo di silicio. Una struttura cristallina per definizione e' una struttura atomica tridimensionale ordinata.

![anisotropic-isotropic](https://user-images.githubusercontent.com/7195133/219942232-0a74399f-18a3-4d56-8053-fea9edabffa5.jpg)

Si intuisce allora dall'immagine che quando si misurano le proprita' di un cristallo si scopre che la misura puo' cambiare in base alla direzione di misurazione e.g. la densita' di protoni, si dice allora che il materiale e' **anisotropo**. Quando invece abbiamo una struttura non ordinata, magari formata da tanti piccoli cristalli, notiamo invece che il materiale presente le stesse misurazioni indipendentemente dalla direzione di misurazione, in quanto le differenze tendono a zero grazie alla disposizione pseudo casuale della materia, si dice allora che il materiale e' **isotropo**.  

![poly-monocrystalline-panel-production](https://user-images.githubusercontent.com/7195133/219941655-c2f66f03-19f3-4a72-a614-95e596b9e1df.jpg)  

Questa e' quindi la differenza sostanziale tra pannelli monocristallini e policristallini, ovvero il modo con cui il wafer di silicio e' stato realizzato: o da un singolo cristallo, quindi **monocristallino**, o da un inisieme di tanti piccoli frammenti di cristallo, quindi **policristallino**.  

## Pannelli a film sottile  

...