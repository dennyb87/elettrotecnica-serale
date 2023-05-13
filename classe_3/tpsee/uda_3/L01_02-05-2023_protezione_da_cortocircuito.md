# Protezione da cortocircuito  

![potere_di_interruzione](https://github.com/dennyb87/elettrotecnica-serale/assets/7195133/7f87edae-9dc6-4aac-941b-28dea4022e27)  

Ogni interruttore ha una caratteristica chiamata **potere di interruzione**. Questa rappresenta la corrente massima che l'interruttore riesce ad interrompere senza danneggiarsi, e quindi poter essere riutilizzato.  

Lo stesso interruttore puo' avere poteri di interruzione diversi a seconda del contesto in cui si va ad utilizzare e.g. civile $4.5kA$ o industriale $6kA$. La normativa ci dice che il potere di interruzione e' considerato minore in un contesto civile in quanto si tiene conto del fatto che generalmente non c'e' manutenzione periodica, al contrario di un contesto industriale.  


## Sollecitazione termica  

Durante un cortocircuito la corrente causa l'aumento della temperatura del conduttore, il dispositivo di protezione allora non solo deve essere in grado di interrompere il circuito, ma deve farlo in un tempo sufficientemente breve da proteggere il cavo da sollecitazioni termiche che potrebbero danneggiarlo.  

Per fare in modo che terminato il cortocircuito il conduttore non superi la temperatura massima stabilita dalle norme per la buona conservazione del cavo stesso, deve essere soddisfatta la seguente condizione:  

$\int_{t_0}^{t_n}i^2dt \le K^2S^2$  

